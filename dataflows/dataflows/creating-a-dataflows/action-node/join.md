# Join

This node is used to connect two data branches together.

<figure><img src="../../../../.gitbook/assets/image (1758).png" alt=""><figcaption></figcaption></figure>

## Keep rows

Includes 2 dropdown lists, each dropdown list corresponds to 1 of the 2 nodes that are connected to the Join node

* Dropdown list includes 2 options:&#x20;
  * All rows: Get all rows of this node&#x20;
  * Matching rows: get only matching rows of this node
* List of possible combinations:



| Matching rows | Matching rows | Inner Join |
| ------------- | ------------- | ---------- |
| All rows      | Matching rows | Left join  |
| Matching rows | All rows      | Right join |
| All rows      | All rows      | Full join  |

## Matching columns

Used to set up join keys between 2 Inputs

## Select column

Used to select which columns of the 2 Inputs are retained after this Join node.

Default selects the first 2 columns in 2 Input

User can search and select the column in each Input to the right

If a column is selected through and there is already another selected column with the same name, it will automatically add #1 after that column name. To make sure there is no column with the same name after this node.

Allow select all/deselect all
