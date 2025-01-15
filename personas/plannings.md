# Plannings

## Overview

Plannings allows the simulation of a result got from a combination of segments.

Without Plannings, it takes more time and resources to build the combination.&#x20;

For example, a journey targets the audiences who&#x20;

* Loyal customers
* Revenue more than $3,000 in 2021
* Didn't make revenue in the first half of 2022
* Made $4,000 in the last half of 2022

_**WIthout Plannings**_

Step 1: Create a loyal customer segment (segment 1)

Step 2: Create the segment for those who made revenue of more than $3,000 in 2021 (segment 2) and include segment 1. The combination of two segments is called segment A

Step 3: Create the segment for those who made a revenue in the first half of 2022 (segment 3). Segment A excludes segment 3 to have segment B

Step 4: Create the segment for those who made $4,000 in the last half of 2022 (segment 4) and include segment B.

_**With Plannings**_

Use Plannings to create the simulation of segment 1, segment 2, segment 3, and segment 4; and explore the final result before actually building it.

### Planning types

There are two types of Plannings

* Customer Plan is used the data of the Customer Business Object to build&#x20;
* Visitor Plan is used the data of the Visitor Business Object to build.

<figure><img src="../.gitbook/assets/image (2554).png" alt=""><figcaption><p>Planning types</p></figcaption></figure>

### Configuration&#x20;

The configuration of a plan includes

* General information has Plan name and Description&#x20;
* Group is the audience segment&#x20;
* The combination logic between Groups includes 'Extend more people' and 'Exclude people'. A plan could have more than one group combined by the logic.

<figure><img src="../.gitbook/assets/image (1511).png" alt=""><figcaption><p>The configuration</p></figcaption></figure>

#### Group&#x20;

[_**Member input method**_](segments.md#details-of-member-input-method) _**and**_ [_**Segment member**_](segments.md#segment-member)

The meaning of these settings are as similar to the settings of a segment.&#x20;

However, Member input method includes Condition and Matching file only.&#x20;

[_**Explore**_ ](plannings.md#explore)

The feature allows creating a statistical report of the group.&#x20;

<figure><img src="../.gitbook/assets/image (2604).png" alt=""><figcaption><p>Explore a Group</p></figcaption></figure>

_**The logic**_&#x20;

A Group could combine with other Groups by including or excluding logic.&#x20;

By clicking the icon, it switches the logic between 'extend more people' and 'exclude people'.

<figure><img src="../.gitbook/assets/image (2420).png" alt=""><figcaption><p>Change the combination logic</p></figcaption></figure>

_**Other actions**_

* ![](<../.gitbook/assets/image (2252).png>) save the settings of a group having two options
  * 'Save as new segment' is to save the Group as a new segment in Segments app
  * 'Load to existing segment' is to replace an existing segment with the settings of the Group&#x20;
* ![](<../.gitbook/assets/image (1915).png>)collapse the settings of a Group

<figure><img src="../.gitbook/assets/image (2339).png" alt=""><figcaption><p>Save and Expand/Collapse the settings of a Group</p></figcaption></figure>

#### The combination logic

The plan has Group A includes Group B excludes Group C. The explanation is

* ![](<../.gitbook/assets/image (2496).png>) Group B means the audiences of Group A include the audiences of Group B
* ![](<../.gitbook/assets/image (1499).png>) Group C means the audiences combined by Group A and Group B exclude the audiences of Group C.

#### Explore

<figure><img src="../.gitbook/assets/image (899).png" alt=""><figcaption><p>Explore of Plannings</p></figcaption></figure>

Explore of Group and Explore of Plan have the same function but&#x20;

* Explore of Group demonstrates the data of a Group
* Explore of Plan demonstrates the data combined by Groups

_**Configuration**_&#x20;

* ![](<../.gitbook/assets/image (1830).png>)is the time CDP 365 created the data of Explore
* ![](<../.gitbook/assets/image (2207).png>)includes 2 options:
  * Private template save the report for the logged-in account
  * Public template save the report for everyone accessing CDP 365
  * Besides, Manage template manages the private templates and public templates. &#x20;
* ![](<../.gitbook/assets/image (741).png>)select charts for the report
* ![](<../.gitbook/assets/image (2350).png>)filter for the report
* The settings of the chart

&#x20;![](<../.gitbook/assets/image (668).png>)

* ![](<../.gitbook/assets/image (1771).png>)a report could have more than one tab. A tab is a page of the report.
