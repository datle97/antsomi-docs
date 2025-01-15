# Initialize customer after submitting form

### 1. Drag block **Optin field** to page design

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdFbW87sjoLAOlPHAMnIFZJ4Lh_jNmh0bx0NW7lyUwR9CLOfIG-w0UDheRHtdlwcW749yP2bsO-fhhUEaS4EHr2_sIHTCDk6TGFrZ2HKnWOcFclAsNFUpHxaylAvOyv2gsdz0OS-bvHDE3QMGFqAuWxA6S-?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 2. Set Id for the fields of the **Optin** block

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcV9oKhf_Dz6KIhgizpLpcDPBybW3og-RGHd972rm8UkCiiGfWJk634XwSmw0kA7pwaJfv42fLQ2Mu4smqN67UCeo6aFjM8WpN59IqEuPRUueR2yOFX19ez0Efgd29FyGWYMBOgBpeJ-4q_h11vukzMKFCs?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 3. In the **Sync data to Event & Business Object** section

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdtpu6dhwSY6aXyjWUZwyrxBhdtzkjq97qsQqusasI3c-2wYNUS_7E1hCJsqQbq1L-QcQ8jz1z_LEfNgFH96os6OBDR0CXBD7z8JQ_gp-jjz-evnHjzYoZLwsNSzzjuOqY-3wo9EZQwQRgINbeKNra8IFFH?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* **Source**: Select the source of the website being delivered
* **Event**: Submit Lead of the source&#x20;

**Note**: If the source does not have an event **Submit lead** and **Identify user**, you must go to the source to add an event **Submit lead** and **Identify user**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfM4d3bcER708F52pqNLAdkt5VJpcG_2wrH-a-N5GxSFH4jAG91j7SVYgmhRE_BSKLIT-fnXVPNn5rWiv5VkFCU2D1nDVY7aHLMkeSeUBmoDZ1MGOevyBvYlYSa4bx46srFBdovEarcbEfQhDxvRIhu3IAU?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* **Attribute Name**: Attributes to receive data after pressing submit

### 4. Setup event in **Success Scripts**

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FsCNBWgG7bCNV9BXOdRHM%2Fimage.png?alt=media&#x26;token=18aa94a1-5116-4a01-8906-be418059c4b4" alt=""><figcaption></figcaption></figure>

* 1 **user** is assigned as Event category
* 2 **indentify** is assigned as Event action
* 3 Get the values ​​of the visitor entered in the fields above and encode it as customer\_id
* 4,5 Get the visitor's values ​​entered in the fields above for customer information

**Result**&#x20;

After clicking submit, the customer will be recorded and saved in the **CDP 365** system

<figure><img src="../../.gitbook/assets/image (3554).png" alt=""><figcaption></figcaption></figure>
