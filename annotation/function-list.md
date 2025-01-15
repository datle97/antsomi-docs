# Function List

## 1. Operator

### 1.1. Plus (+)

Plus sign for addition

### 1.2. Minus (-)

Minus sign for subtraction

### 1.3. Multiply (\*)

Multiply sign for multiplication

### 1.4. Devide (/)

Devide by sign for division

### 1.5. Less than (<)

Returns true if expr 1 is less than expr 2

### 1.6. Greater than (>)

Returns true if expr 1 is greater than expr 2

### 1.7. Less than or equal to (<=)

Returns true if expr1 is less than or equal to expr2

### 1.8. Greater than or equal to (>=)

Returns true if expr1 is greater than or equal to expr2

### 1.9. Equal to (=)

Returns true if expr1 equals expr2, or false otherwise

### 1.10. Less than or greater than but not equal to (<>)

Returns true if expr1 is not equal to expr2, or false otherwise

### 1.11. Not equal to (!=)

Returns true if the operands don't have the same value; otherwise, it returns false

### 1.12. Remainder (%)

Returns the remainder after expr1/expr2

## 2. String

### 2.1. Char

Converts a numeric value between 0 and 255 to the character value corresponding to the ASCII code.

_**CHAR(expr)**_

* expr is any expression that evaluates to a numerical value between 0 and 255.

### 2.2. Length

Returns the length, in number of characters, of a specified string. The length is returned excluding any trailing blank characters.

_**LENGTH(expr)**_

* expr is any expression that evaluates to a character string

### 2.3. Trim

Removes the leading and trailing space characters from string

_**TRIM(expr)**_

* expr is any expression that evaluates to a character string.

## 3. Math

### 3.1. Abs

Calculates the absolute value of a numeric expression.&#x20;

_**ABS(expr)**_

* expr is any expression that evaluates to a numerical value.

### 3.2. Rand

Returns a pseudo-random number between 0 and 1

### 3.3. Round

Rounds a numeric expression to n digits of precision.

_**ROUND(expr, integer)**_

* expr is any expression that evaluates to a numerical value.
* integer is any positive integer that represents the number of digits of precision.

### 3.4. Sqrt

Calculates the square root of the numeric expression argument. The numeric expression must evaluate to a nonnegative number.

## 4. Calendar/ Date

### 4.1. Current\_Time

Returns the current time to the specified number of digits of precision, for example: HH:MM:SS.SSS

_**CURRENT\_TIME**_

If no argument is specified, the function returns the default precision.

### 4.2. DayOfWeek

Returns a number between 1 and 7 corresponding to the day of the week for a specified date expression.

For example, 1 always corresponds to Sunday, 2 corresponds to Monday, and so on through to Saturday which returns 7.

### 4.3. Hour

Returns a number (between 0 and 23) corresponding to the hour for a specified time expression. For example, 0 corresponds to 12 a.m. and 23 corresponds to 11 p.m.

### 4.4. Minute

Returns a number (between 0 and 59) corresponding to the minute for a specified time expression.

### 4.5. Month

Returns the number (between 1 and 12) corresponding to the month for a specified date expression.

### 4.6. Second

Returns the number (between 0 and 59) corresponding to the seconds for a specified time expression.

### 4.7. Year

Returns the year for the specified date expression.

### 4.8. Now

Returns the current timestamp. The NOW function is equivalent to the CURRENT\_TIMESTAMP function.

### 4.9. Week\_Of\_Year

Returns a number (between 1 and 53) corresponding to the week of the year for the specified date expression.

## 5. Expressions

### 5.1. Case

This form of the Case statement evaluates each WHEN condition and if satisfied, assigns the value in corresponding THEN expression.&#x20;

If none of the WHEN conditions are satisfied, it assigns the default value specified in the ELSE expression.&#x20;

If no ELSE expression in specified, the system will automatically add an ELSE NULL. CASE WHEN request\_condition1 THEN expr1 ELSE expr2 END exprs is any valid expression

\


