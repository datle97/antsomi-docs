---
description: >-
  If you intend to employ Python code within the dataflow for data
  transformation before exporting it from CDP 365, this document will be
  beneficial to you.
---

# Script

## Step 1: Add the Script node to your dataflow

For reference to the node, please consult the image provided below:

<figure><img src="../../../../.gitbook/assets/image (2698).png" alt=""><figcaption><p>Add the Script node</p></figcaption></figure>

_**Note:** After the Script node cannot add another node._

## Step 2: Write your Python code

It has 3 zones:

* Zone **1** outlines the attributes prepared for transformation
* Zone **2** places your Python code within it
* Zone **3** involves modifying the coding theme and default fields of CDP 365.

<figure><img src="../../../../.gitbook/assets/image (2699).png" alt=""><figcaption><p>Write Python code</p></figcaption></figure>

For reference to the transforming result, please consult the code below:

```python
import pandas
import sys

# Load data from system
df = pandas.read_csv(sys.argv[1])

# The following code to create a dataframe and remove duplicated rows is always executed and acts as a preamble for your script: 
dataset = pandas.DataFrame(df)
dataset = dataset.drop_duplicates()

# Paste or type your script code here:

print(dataset)
```

## Step 3: Preview the transformed data

Before executing the code, it's essential to preview it beforehand to **ensure that the data is prepared for transformation within the Script node**.&#x20;

Kindly click the "**Preview**" button for this purpose.

<figure><img src="../../../../.gitbook/assets/image (2700).png" alt=""><figcaption><p>Preview the data</p></figcaption></figure>

## Step 4: Test the Script node

Once you've successfully previewed the data and confirmed its accuracy, you can proceed to run the code. Kindly click the "**Test**" button to do so.

<figure><img src="../../../../.gitbook/assets/image (2701).png" alt=""><figcaption><p>Run the code</p></figcaption></figure>

## Step 5: Check the running status

Upon executing the code, a banner will appear from the **lower-left corner** of your screen. Kindly inspect this banner to monitor the **status** of the execution.

### In case of successful running

<figure><img src="../../../../.gitbook/assets/image (2702).png" alt=""><figcaption><p>Success test</p></figcaption></figure>

### In case of failed running

<figure><img src="../../../../.gitbook/assets/image (2703).png" alt=""><figcaption><p>Failed test</p></figcaption></figure>

_**Note:** After the Script node cannot add another node._
