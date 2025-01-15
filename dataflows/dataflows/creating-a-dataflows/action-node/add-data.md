# Add data

Set input data for dataflow.

<figure><img src="../../../../.gitbook/assets/image (2220).png" alt=""><figcaption></figcaption></figure>

Automatically add 1 Add data node when starting to create Dataflow. Multiple Add Data nodes can be added to 1 Dataflow.

The details of an Add data node are as follows:

<figure><img src="../../../../.gitbook/assets/image (2118).png" alt=""><figcaption></figcaption></figure>

## Data Source

Data sources with a Connected state can be selected.

The first Add data node when starting to create Dataflow will default to the initially selected datasource.

## Using Aggregation

Used to specify whether or not to group by data lines with duplicate data.

## Available fields

List of fields available in the currently selected Datasource

## Condition

Set data filtering conditions at the Add data node

_**Note:**_ After clicking Datasource will proceed to create a new Add Data node and a Join node to connect the new Add Data to the current branch. And will focus on this Join node after selecting Datasource
