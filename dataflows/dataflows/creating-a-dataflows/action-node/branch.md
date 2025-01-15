# Branch

Use to branch out many data processing branches. All these branches will have the same Data output

<figure><img src="../../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>

Users can create more branches or delete branches in the node detail interface

<figure><img src="../../../../.gitbook/assets/image (1183).png" alt=""><figcaption></figcaption></figure>

When the User clicks Delete after each branch, it will delete the entire branch in the node diagram regardless of whether the branch has a node behind the branch or not.

* When deleting only 1 branch, it will automatically delete this branch node and the remaining branch will continue to replace the node branch.
* When a branch is deleted, it will renumber the branches below that deleted branch. For example, there are 5 branches numbered 1,2,3,4,5, when deleting branch 3 --> branch 4 will rename to 3 and branch 5 will rename to 4.&#x20;
* If the User deletes branch 1, it will push the nodes in branch 2 up as usual.

Maximum allowed to create 5 branches --> Hide Add branch button when creating 5 branches and only show again when at least 1 branch is deleted
