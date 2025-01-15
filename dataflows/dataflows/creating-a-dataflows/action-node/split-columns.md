# Split Columns

Used to split (split) data of a column into 1 or more different columns. Can split based on position (position) or based on separator character (delimiter)

<figure><img src="../../../../.gitbook/assets/image (1358).png" alt=""><figcaption></figcaption></figure>

* Split column: Used to select the column you want to split data
* On: Used to specify how the selected Column data is split
* Delimiter: Used to specify which character will be the symbol to separate the data between the preceding and following parts of that character
* Occurrence: Used to specify the first extracted data to be taken from the beginning to the position of the delimiter character in the original data.
* Number of parts to create: Used to specify the number of columns to be created after the split. If a cell has no data, it will be null --> can create a column where all data is null.
* Column list: Used to input column name for the generated columns. The number of lines here will depend on the option entered in Number of parts to create.
