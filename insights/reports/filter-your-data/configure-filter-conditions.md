---
description: >-
  Filters conditions tell Insights which records to include in or exclude from
  your report.
---

# Configure filter conditions

## Configure filter conditions

Filters conditions tell Insights which records to include in or exclude from your report.

### Include vs Exclude filters

_Include_ filters retrieve only the records that match the conditions, while _exclude_ filters retrieve only the records that DON'T match the conditions.

### Filter clauses

Conditions consist of one or more clauses.

A simple filter has just one clause. For example, `Country` **Equals** "France".

Multiple clauses can be joined with "OR" logic (true if any conditions are met), "AND" logic (true if all conditions are met), or both. For example:`Country` **Equals** "France" OR`Country` **Equals** "Germany"AND`User Type` **Equals** "New user"AND`Sessions` **Greater Than** 100

An OR clause can contain dimensions or metrics, but not both.

### Operators <a href="#operators" id="operators"></a>

Operators compare the fields in the filter against values you provide. The operators available depend on whether you are filtering a text, number, date, or logical field.

### Text operators

| Operator    | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Is          | <p>The comparison value exactly matches the dimension value.</p><p><strong>Example</strong></p><p>The comparison value "chrome" exactly matches "chrome" but not "Chrome" or "chromebook"</p>                                                                                                                                                                                                                                                                                                                                   |
| Contains    | <p>The comparison value is contained within the dimension value.</p><p><strong>Example</strong></p><p>The comparison value "chrome" is contained within "chrome" and "chromebook" but not "Chrome"</p>                                                                                                                                                                                                                                                                                                                          |
| Starts with | <p>The dimension value starts with the comparison value.</p><p><strong>Example</strong></p><p>The comparison value "Chrome" starts "Chrome" and "Chromebook" but not "Google Chrome"</p>                                                                                                                                                                                                                                                                                                                                        |
| Matches any | <p>One or more of the comparison values exactly matches the dimension value. Works just like Equals but for a comma-separated list of values.</p><p><strong>Example</strong></p><p>IN "Chrome,Windows,MacOS" matches if any of those are in the dimension.</p><p>If your values contain commas or backslashes as part of the data to match, use a backslash to escape them.</p><p><strong>Example</strong></p><p>If you want to match "ab,cd" and "50\50" precede the comma and backslash with \:</p><p>In "ab\,cd, 50\\50"</p> |
| Is Null     | Matches if the dimension value is null.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

### Numeric operators

| Operator                        | Description                                                                    |
| ------------------------------- | ------------------------------------------------------------------------------ |
| Equals ("=")                    | The dimension or metric value is equal to the comparison value                 |
| Less than ("<")                 | The dimension or metric value is less than the comparison value                |
| Greater than (">")              | The dimension or metric value is greater than the comparison value             |
| Greater than or equal to (">=") | The dimension or metric value is greater than or equal to the comparison value |
| Less than or equal to ("<=")    | The dimension or metric value is less than or equal to the comparison value    |
| Is Null                         | The dimension or metric value is null                                          |

### Date operators

| Operator | Description                                                |
| -------- | ---------------------------------------------------------- |
| After    | The dimension value is greater than the comparison value   |
| Between  | Dimension values are within the range of comparison values |
| Before   | The dimension value is less than the comparison value      |
| Is Null  | The dimension value is null                                |
