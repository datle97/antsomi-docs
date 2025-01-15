# Basic

<figure><img src="../../../../.gitbook/assets/image (3810).png" alt=""><figcaption></figcaption></figure>

## View Styling

<figure><img src="../../../../.gitbook/assets/image (3798).png" alt=""><figcaption></figcaption></figure>

### **Campaign Width**:&#x20;

* The container width can be customized to a specific **pixel** or **percentage** value

{% hint style="info" %}
On mobile devices, you should adjust 100% of the screen width
{% endhint %}

### **Background setting**

#### **Background color:**&#x20;

Applies background color of the template.

<figure><img src="../../../../.gitbook/assets/image (3800).png" alt=""><figcaption></figcaption></figure>

#### **Background image**

You can choose the image by clicking ![](<../../../../.gitbook/assets/image (3801).png>)

<figure><img src="../../../../.gitbook/assets/image (3802).png" alt=""><figcaption></figcaption></figure>

* _**Image URL**_: A web address that specifies the location of an image
* _**Image Position**_: The position of the background image such as left top, left center, right top, right center, etc.
* _**Image Repeat**_: Sets how background images are repeated (Repeat, Repeat horizontal, repeat vertical, etc.)
* _**Image Size**_: How an image should be resized to fit its container
  * _**Contain**_: The image keeps its aspect ratio but is resized to fit within the given dimension
  * _**Cover**_: The image keeps its aspect ratio and fills the given dimension. The image will be clipped to fit
  * _**Auto**_: The image keeps its aspect ratio and fills the given dimension automatically

## **Content Sources Settings**

<figure><img src="../../../../.gitbook/assets/Template Setting – Business Objects.png" alt=""><figcaption></figcaption></figure>

* Get information fields matching your needs and display them in the campaign. For example, if you design a pop-up showing the most viewed product, create a Group that has Product Data Object as its content source, then it will get data from Product.

<figure><img src="../../../../.gitbook/assets/image (3803).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (3804).png" alt=""><figcaption></figcaption></figure>

* Each Data Object has its configuration
  1. _**Product**_:
     * _**Filter**_: Filter desired data, you can also combine conditions such as AND/OR&#x20;
     *   _**Ranking**_:

         * _**Algorithms**_

         <figure><img src="../../../../.gitbook/assets/image (3805).png" alt=""><figcaption></figcaption></figure>

         * _**Sort**_: Sort by order or mix. In sort by order, you can drag and drop to arrange&#x20;
         * _**Add Algorithms**_: "_**Seen product**_" is the default algorithms
           * _**Viral products**_: Products in collectors want to viral
           * _**Seen products**_: Products the user has already browsed
           * _**Carted**_: Product this user has already placed in the shopping cart (and which are still there)
           * _**Bought**_: Products this user recently bought
           * _**Recency**_: Products with a recent release or availability date
           * _**Same category**_: Products in the same category as the current product
           * _**Same brand**_: Products in the same brand as the current product
           * _**Look-alike products**_: Products that have a similar context in the title description to the current product
           * _**Product bought most often**_: Products most often bought during the chosen time frame
           * _**Product carted most often**_: Products most often carted during the chosen time frame
           * _**Product viewed most often**_: Products most often viewed during the chosen time frame
           * _**Frequently bought together**_: Product usually bought with current product
           * _**Frequently cart together**_: Product usually adds to a cart with the current product
           * _**Frequently seen together**_: Product usually seen with current product
           * _**Distance**_: Products that satisfy the conditions of comparison between two attributes in a range of value
           * _**Similarity bought**_: Products usually bought with the last products the current user bought
           * _**Similarity cart:**_ Products usually add a cart with the last products of the current user carted
           * _**Similarity seen**_: Products usually seen with the last products of the current user seen
           * _**Retarget search**_: Product the user searched for
           * _**Same interest**_: Products in the same categories as those the user has shown the most interest in
         * _**Excluded:**_ The feature allows you to hide the filtered information of the product

         <figure><img src="../../../../.gitbook/assets/image (3806).png" alt=""><figcaption></figcaption></figure>

         * _**Custom:**_ It allows you to custom algorithms

         <figure><img src="../../../../.gitbook/assets/image (3807).png" alt=""><figcaption></figcaption></figure>
     *   _**Fallback**_: Fallback items that are always recommended in case there are no recommendations that can be presented

         * _**Hidden**_: Hide the template in case there are no recommendations
         * _**None**_: Shows recommendations that satisfied the algorithms
         * _**Most seen**_: Recommendations items that were most frequently seen
         * _**Most cart**_: Recommendations items that were most frequently added to the cart
         * _**Most bought**_: Recommendations items that were most frequently bought

         <figure><img src="../../../../.gitbook/assets/image (3808).png" alt=""><figcaption></figcaption></figure>
  2. **Others:**
     * _**Filter:**_ Filter desired data, you can also combine conditions such as AND/OR&#x20;
     * _**Custom Ranking**_: It allows you to custom algorithms

## **Tracking Module**

<figure><img src="../../../../.gitbook/assets/image (3809).png" alt=""><figcaption></figcaption></figure>

* _**UTM\_Source**_: This indicates the social network, search engine, newsletter name, or other specific source driving the traffic. _**Examples**_: facebook, twitter, blog, newsletter, etc
* _**UTM\_Medium**_: This tracks the type of channel driving the traffic: organic social, paid social, email, and so on. _**Examples**_: cpc, organic\_social
* _**UTM\_Campaign:**_ Give each campaign a name so you can keep track of your efforts. This could be the product name, a contest name, a code to identify a specific sale or promotion, an influencer ID or a tagline. **Examples:** summer\_sale, free\_trial
* _**UTM\_Term:**_ Use this UTM tag to track paid keywords or key phrases. _**Examples:**_ social\_media, newyork\_cupcakes
* _**UTM\_Content:**_ This parameter allows you to track different ads within a campaign. _**Examples:**_ video\_ad, text\_ad, blue\_banner, green\_banner
