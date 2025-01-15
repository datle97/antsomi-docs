# Set up Event Tracking code to track events into CDP

## **I. MAIN SCRIPT**

Add this script to the header tag of all the website pages that you want to track events (similar to what you have done with Google Analytics JS or Facebook Pixel JS.)

Example:

```
<!-- ANTSOMI SDK Analytics script -->
<script type = "text/javascript" >
   var _portalId = "PORTAL_ID"; // Your Portal ID 
   var _propId = "PROPERTY_ID"; // Your Website Property ID
   var _CDP_DELIVERY_TRIGGER=true;
(function() {
    var w = window;
    if (w.web_event) return;
    var a = window.web_event = function() {
        a.queue.push(arguments);
    }
    a.propId = _propId;
    a.track = a;
    a.queue = [];
    var e = document.createElement("script");
    e.type = "text/javascript", e.async = !0, e.src = "//st-a.cdp.asia/insight.js";
    var t = document.getElementsByTagName("script")[0];
    t.parentNode.insertBefore(e, t)
})(); </script>
<!-- End of ANTSOMI SDK Analytics script -->
```

#### How to get Main Script in CDP

1. Log into the **CDP** system
2. Go to menu: **DATA HUB -> Event Sources**

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F7eWUmnqEl7t5uZjKhUxQ%2Fimage.png?alt=media&#x26;token=7acd6123-62d7-4473-8e25-e48d141c1b5b" alt=""><figcaption></figcaption></figure>

3\. Select "Websites" Source, then go to "Setting" tab. You will be Main Script

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FjLvBvAZkqn92g6166HqV%2Fimage.png?alt=media&#x26;token=b01d6e77-ef49-44ae-a6a9-4499a0fd9d4b" alt=""><figcaption></figcaption></figure>

## **II -  EVENTS TRACKING**

<table><thead><tr><th width="78">No</th><th>Event</th><th>Dimension</th><th width="126">Event Type</th><th width="106">Required</th><th>Trigger</th></tr></thead><tbody><tr><td>1</td><td>Pageview / setPageConfig</td><td><ul><li>page_type</li><li>page_category</li></ul></td><td><strong>Default</strong></td><td><strong>Yes</strong></td><td><ul><li>Default by SDK</li><li>Add to head tag all pages</li><li>set _cdp365Analytics</li></ul></td></tr><tr><td>2</td><td>Product View</td><td><ul><li>item: product</li></ul></td><td><strong>Ecommerce</strong></td><td><strong>Yes</strong></td><td>​Page loaded, User viewed a product details</td></tr><tr><td>3</td><td>Add to cart</td><td><ul><li>item: product</li></ul></td><td><strong>Ecommerce</strong></td><td><strong>Yes</strong></td><td>User added a product to their shopping cart</td></tr><tr><td>4</td><td>Remove from Cart</td><td><ul><li>item: product</li></ul></td><td><strong>Ecommerce</strong></td><td><strong>Yes</strong></td><td>User removed a product to their shopping cart</td></tr><tr><td>5</td><td>Cart view</td><td><ul><li>item: product</li></ul></td><td><strong>Ecommerce</strong></td><td><strong>Yes</strong></td><td>The user viewed their shopping cart</td></tr><tr><td>6</td><td>Cart checkout</td><td><ul><li>item: product</li></ul></td><td><strong>Ecommerce</strong></td><td><strong>Yes</strong></td><td>User-initiated the order process (a transaction is created)</td></tr><tr><td>7</td><td>Purchase</td><td><ul><li>item: product</li></ul></td><td><strong>Ecommerce</strong></td><td><strong>Yes</strong></td><td>User purchased and completed the order on the thank you page</td></tr><tr><td>8</td><td>Product Search</td><td><ul><li>item: product</li></ul></td><td><strong>Ecommerce</strong></td><td><strong>Yes</strong></td><td>User searched for products by keyword</td></tr><tr><td>9</td><td>User sign-In</td><td></td><td></td><td></td><td>User signed successful</td></tr><tr><td>10</td><td>User sign-Up</td><td></td><td></td><td></td><td>User signed successful</td></tr></tbody></table>

## **III -  EVENTS TRACKING CODE**

### **1. Pageview / setPageConfig:**

```
<script>
  var _cdp365Analytics = {
       first_party_domain: ".magento.antsomi.com",
       page: {"page_type": "Home",
             "page_category": "Home"
       }
   };
</script>
```

**Code sample:**

Event trigger:  Page loaded and add to head tag all pages

### **2. Product category page:**

* **page\_type :** Fixed value to **"category" (required)**
* **page\_category :** The current category name. **(required)**
* **items:** Top 5 highlight products **(required)**

Sample code tracking for the category page

```
<script>
  var _cdp365Analytics = {
 first_party_domain: ".magento.antsomi.com",
       page: {"page_type": "category",
             "page_category": "Men"
       },
	 items: [{
            "type":"product",
            "sku":"16171312",
            "page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
            "image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
            "name":"áo thun nam",
            "id":"1311721",
            "price":179000,
            "original_price":17000
            "brand":"Aristino"
            "size": "39"
            "color": "black"
            "main_category":"Men",
            "category_level_1":"",
            "category_level_2":""
            },{
            "type":"product",
            "sku":"16171312",
            "page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
            "image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
            "name":"áo thun nam",
            "id":"1311721",
            "price":179000,
            "original_price":17000
            "brand":"Aristino"
            "brand":"Aristino"
            "size": "39"
            "color": "black"
            "main_category":"Men",
            "category_level_1":"",
            "category_level_2":""
            }]
   }; 
  
</script>
```

* **type, id,**  and **name** are required params
* The other params are optional, but there are a number of params that are required to serve the recommended product:
  * price
  * main\_category
  * category\__level\__&#x31;
  * category\__level\__&#x32;
  * brand

### **3. Product detail page + product view**

**page\_type:** Fixed value to **"**&#x70;roduct\_detai&#x6C;**" (required)**

**page\_category:** The current category name of the product that you are viewing. **(required)**

**items:**  The product detail **(required)**

Sample code tracking for the **Product detail page + product view**

```
<script>
  var _cdp365Analytics = {
 first_party_domain: ".magento.antsomi.com",
       page: {"page_type": "product_detail",
             "page_category": "Men"
       },
	 items: [{
            "type":"product",
            "sku":"16171312",
            "page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
            "image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
            "name":"áo thun nam",
            "id":"1311721",
            "price":179000,
            "original_price":17000
            "brand":"Aristino"
            "size": "39"
            "color": "black"
            "main_category":"Men",
            "category_level_1":"",
            "category_level_2":""
            }],
            track: [['product', 'view']]
   }; 
  
</script>

```

* **type, id,**  and **name** are required params
* The other params are optional, but there are a number of params that are required to serve the recommended product:
  * price
  * main\_category
  * category\__level\__&#x31;
  * category\__level\__&#x32;
  * brand

### **4. Cart page + Cart view**

User viewed product shopping cart

* **page\_type :** Fixed value to **"cart" (required)**
* **page\_category :** Fixed value to **"cart" (required)**

Sample code tracking for the category page

<pre><code>&#x3C;script>
<strong> var _cdp365Analytics = {
</strong> first_party_domain: ".magento.antsomi.com",
       page: {"page_type": "cart",
             "page_category": "cart"
       },
	 items: [{
      "type":"product",
      "sku":"16171312",
      "page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
      "image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
      "name":"áo thun nam",
      "id":"1311721",
      "price":179000,
      "original_price":17000
      "brand":"Aristino"
      "size": "39"
      "color": "black"
      "main_category":"Men",
      "category_level_1":"",
      "category_level_2":""
      },{
      "type":"product",
      "sku":"16171312",
      "page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
      "image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
      "name":"áo thun nam",
      "brand":"Aristino"
      "id":"1311721",
      "price":179000,
      "original_price":17000
      "size": "39"
      "color": "black"
      "main_category":"Men",
      "category_level_1":"",
      "category_level_2":""
      }],
	 track: [['product', 'view_cart']]		
   };
&#x3C;/script>

</code></pre>

* **type, id,**  and **name** are required params
* The other params are optional, but there are a number of params that are required to serve the recommended product:
  * price
  * main\_category
  * category\__level\__&#x31;
  * category\__level\__&#x32;
  * brand

### **5. Product search results page  + product search events**

* **page\_type :** Fixed value to **"search" (required)**
* **page\_category :** Fixed value to **"search results" (required)**
* **src\_search\_term:**  Search text keyword. **(required)**
* **Items: (required)**
  * id : Product SKU , differentiate by  Variant size

```
<script>
  var _cdp365Analytics = {
  first_party_domain: ".magento.antsomi.com",
	 page: {"page_type": "search", "page_category": "search results"},
	items: [{
		"type":"product",
		"sku":"134171312",
		"page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
		"image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
		"name":"áo thun nam xanh",
		"id":"13327230",
		"price":179000,
		"original_price":17000
		"brand":"Aristino"
		"size": "39"
                "color": "black"
		"main_category":"Men",
		"category_level_1":"",
		"category_level_2":""
		},{
		"type":"product",
		"sku":"17371312",
		"page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
		"image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
		"name":"áo thun nam đen",
		"brand":"Aristino"
		"size": "39"
                "color": "black"
		"id":"1821712",
		"price":179000,
		"original_price":17000
		"main_category":"Men",
		"category_level_1":"",
		"category_level_2":""
	}],
	  track: [['browsing', 'product_search' , {extra: {"src_search_term": "áo thun"}}]]		
   };
</script>

```

* **type, id,**  and **name** are required params
* The other params are optional, but there are a number of params that are required to serve the recommended product:
  * price
  * main\_category
  * category\__level\__&#x31;
  * category\__level\__&#x32;
  * brand

### **6. Thank you page + purchase event**



* **page\_type :** Fixed value to **"checkout" (required)**
* **page\_category :** Fixed value to **"thank\_you" (required)**
* **customer\_id :** will be the primary key in CDP. **(required)**
  * Example : MD5(phone\_number), md5(email\_address), …, etc
* **quantity:** Product quantity **(required)**
* **is\_web:**  Fixed value is **true (required)**
* **payment\_method:** an option of values **'OTC**' ,…, etc **(required)**
* **Items: (required)**
  * id : Product SKU , differentiate by  Variant size

```
<script>
  var _cdp365Analytics = {
 first_party_domain: ".magento.antsomi.com",
	 page: {"page_type": "checkout", "page_category": "thank_you"},
	 items: [{
            "type":"product",
            "sku":"134171312",
            "page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
            "image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
            "name":"áo thun nam xanh",
            "id":"13327230",
            "price":179000,
            "original_price":17000
            "quantity":1
            "brand":"Aristino"
            "size": "39"
            "color": "black"
            "main_category":"Men",
            "category_level_1":"",
            "category_level_2":""
            },{
            "type":"product",
            "sku":"134171312",
            "page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
            "image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
            "name":"áo thun nam xanh",
            "id":"13327230",
            "size": "39"
            "color": "black"
            "brand":"Aristino"
            "quantity":2
            "price":179000,
            "main_category":"Men",
            "category_level_1":"",
            "category_level_2":""
      }],
     extra: {
        order_id: "XXX",
        revenue: 100000.0,
        discount_amount: 0.0,
        voucher_code: "YYYY",
        customer_id: "73271090fe10d41bf93c55765376", // md5(phone)
        identify_event: "Purchase",
        customer_name: "Barack Obama",
        email: "obama @gmail.com", 
        phone: "09123123123",
        is_web: true, 
        purchase_time: "2021-09-13 23:50:00",
        payment_method: 'OTC'
    },
    track: [['product', 'purchase']]	
};

</script>
```

* **type, id,**  and **name** are required params
* The other params are optional, but there are a number of params that are required to serve the recommended product:
  * price
  * main\_category
  * category\__level\__&#x31;
  * category\__level\__&#x32;
  * brand

### **7. Add to cart**

**Items:  (required)**

* id : Product SKU , differentiate by  Variant size

```
<script>
   $( "#ADD_TO_CART_BUTTON" ).click(function( event ) {
      web_event.track('product', 'add_to_cart', {
  items: [{
   "type":"product",
   "sku":"134171312",
   "page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
   "image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
   "name":"áo thun nam xanh",
   "id":"13327230",
   "brand":"Aristino"
   "size": "39"
   "original_price":17000
   "color": "black"
   "price":179000,
   "main_category":"Men",
   "category_level_1":"",
   "category_level_2":"",
   "quantity":1
}]
 });
   });
</script>

```

* **type, id,**  and **name** are required params
* The other params are optional, but there are a number of params that are required to serve the recommended product:
  * price
  * main\_category
  * category\__level\__&#x31;
  * category\__level\__&#x32;
  * brand

### **8. Remove from cart**

* **type: "product".** fix this value **(required)**
* **Items: (required)**
  * id : Product SKU , differentiate by  Variant size

```
<script>
   $( "#REMOVE_CART_BUTTON" ).click(function( event ) {
 web_event.track('product', 'remove_cart', {
   items: [{
        type: "product",
              id: "10211124", // product_sku ( variant_id)
        quantity: 1
    }]
 });
   });
</script>
```

### **9. Cart checkout**



* **customer\_id :** will be the primary key in CDP.  **(required)**
  * Example : MD5(phone\_number), md5(email\_address), …, etc
* **payment\_method:** an option of values **'OTC**' ,…, etc **(required)**
* **Items: (required)**
  * id : Product SKU , differentiate by  Variant size

<pre><code>&#x3C;script>
   $( "#CHECKOUT_FORM" ).submit(function( event ) {
      // code tracking here 
    web_event.track('product', 'checkout', {
     items: [{
<strong>		"type":"product",
</strong>		"sku":"134171312",
		"page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
		"image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
		"name":"áo thun nam xanh",
		"id":"13327230",
		"quantity":1,
		"size": "39"
                "color": "black"
                "brand":"Aristino"
		"price":179000,
		"original_price":17000
		"main_category":"Men",
		"category_level_1":"",
		"category_level_2":""
    }, {
		"type":"product",
		"sku":"134171312",
		"page_url":"https://magento.antsomi.com/men/tops-men/tees-men.html",
		"image_url":"https://magento.antsomi.com/media/catalog/product/cache/a3591e0b9f4456c1928a5351b0f7341e/m/s/ms08-black_main_1.jpg",
		"name":"áo thun nam xanh",
		"id":"13327230",
		"brand":"Aristino"
		"quantity":1,
		"size": "39"
                "color": "black"
		"price":179000,
		"original_price":17000
		"main_category":"Men",
		"category_level_1":"",
		"category_level_2":""
    }],
     dims: {
     	   customers : {
            customer_id: "26312561290fe10d41bf93c55765376", // md5(phone)
  	    customer_name : "Barack Obama",
  	    email: "obama@gmail.com", 
  	    phone: "09123123123",
  	    address: "Address 1",
  	    district: "District 1",
  	    city: "City Name",
  	    date_created: '2022-08-01 13:50:00',  // yyyy-MM-dd 
            identify_event: "checkout", //  fix value
     	    }
     },
     extra: {     
            payment_method: 'OTC',
            delivery_method: 'antsomi giao hàng',
            voucher_code: "YYYY" // The  voucher code applied or empty
       }       
     });
   });
&#x3C;/script>
</code></pre>

* **type, id,**  and **name** are required params
* The other params are optional, but there are a number of params that are required to serve the recommended product:
  * price
  * main\_category
  * category\__level\__&#x31;
  * category\__level\__&#x32;
  * brand

### **10. User Sign-In**

Event trigger: After the user login is successful.

* **customer\_id :** will be the primary key in CDP. **(required)**
  * Example : MD5(phone\_number), md5(email\_address), …, etc
* **identify\_event: 'sign\_in' .** Fix this value **(required)**
* **customer\_name (required)**

```
web_event.track('user', 'sign_in', {
    extra:{
	customer_id: "2891b0086090fe10d41bf93c55765376", 
        customer_name: 'Barack Obama',
        phone: '09123123123', 
        email: 'nguyenvana@gmail.com', 	
        identify_event: 'sign_in' 
    }    
})
```

### **11. User Sign-up**

Event trigger: After the user sign-up is successful.

* **customer\_id :** will be the primary key in CDP.&#x20;
  * Example : MD5(phone\_number), md5(email\_address), …, etc
* **identify\_event: 'sign\_up' .** Fix this value
* **customer\_name (required)**

```
web_event.track('user', 'sign_up', {
    extra:{
        customer_id: "2891b0086090fe10d41bf93c55765376", 
    	customer_name: 'Barack Obama', 
        phone: '09123123123', 
        email: 'nguyenvana@gmail.com',
        identify_event: 'sign_up' 
    }    
})
```

### 12. User Sign-out

When the user logout

```
web_event.track('user', 'sign_out');
```

### 13. **Lead Form Submit and User Identify**

Track a both of events when user submited form successfully&#x20;

Set value for leadData with parameters exactly in code sample.

**type, id,  phone,** and **name** are required params

```
<script>
jQuery("#targetForm").on("submit", function() {
    var leadData = {
        type: "lead", // required and fix this value
        name: 'Nguyen van A', // required 
        phone: '09122323233', // required 
        email: 'nguyenvana@gmail.com',
        city: 'Hồ Chí Minh',
        district: 'Quận 1',
        ward: '12',
        address: '122/19 Nguyễn Huệ',
        lead_time: '2022-04-06 22:40:00', // time to submit . format: yyyy-MM-dd HH:mm:ss 
        lead_locate: window.location.href,
        lead_event: 'Event sale sinh nhật' // Event name for each landing page .
    };

    console.log('cdp leadData:', leadData);

    var properties = {
        items: [leadData]
    };

    //event lead form 
    web_event.track('lead_form', 'submit', properties);

    // call to user identify event  (can use this function)
     _cdpUserIdentifyFromLead(leadData);

});

function _cdpUserIdentifyFromLead(leadData) {

    if (typeof leadData != 'object') {
        console.log('no tracking identify_event from lead:', leadData);
        return;
    }

    if (leadData.phone == undefined || leadData.phone == '' || leadData.phone.length < 9) {
        console.log('Phone Check. no tracking identify_event from lead:', leadData);
        return;
    }

    if (leadData.name == undefined || leadData.name == '') {
        console.log('Name check. no tracking identify_event from lead:', leadData);
        return;
    }

    if (leadData.email == undefined || leadData.email == '' || leadData.email.indexOf('@') <= 0) {
        console.log('Email Check. no tracking identify_event from lead:', leadData);
        return;
    }

    var extraData = leadData || {};

    extraData.is_lead = true;
    extraData.is_ecom = true;
    extraData.lead_source = 'landing page';
    extraData.identify_event = 'lead form LP';
    extraData.phone_number = leadData.phone;
    extraData.customer_name = leadData.name;

    if (leadData.phone != undefined && leadData.phone != '' &&
        window._cdpEventFunction != undefined &&
        typeof window._cdpEventFunction.md5 == 'function') {
        extraData.customer_id = window._cdpEventFunction.md5(leadData.phone);
    }

    console.log('cdp identify data:', extraData);

    var properties = {
        extra: extraData
    };

    //properties
    web_event.track('user', 'identify', properties);

}
</script>

```

## **IV. BLOG TRACKING EVENTS**

### &#x20;**1. Blog Category**

Add this script to the header tag of the all blog pages - bellow the main code

**page:**

&#x20;  \+ **page\_type:** Fixed value to **"article" (required)**

&#x20;  \+ **page\_category:** The current article category name. **(required)**

**Code sample**

```
<!-- Antsomi CDP 365  script -->
<script type="text/javascript">
var _cdp365Analytics = {       
	 page: {"page_type": "article", "page_category": "<The current article category name>"}           
}
</script>
```

### **2. Blog Detail**

Add this script to the header tag of the all blog pages - bellow the main code

Item product list size: The main article detail.

User viewed article details

**page:**

&#x20;  \+ **page\_type:** Fixed value to **"article\_detail" (required)**

&#x20;  \+ **page\_category:** The current article category name. **(required)**

**items:**

&#x20;   **+ type :** Fixed value to **"article" (required)**

&#x20;   **+ id:** Article ID **(required)**

&#x20;   **+ name:** Article Title **(required)**

**Code sample**

```
<!-- Antsomi CDP 365  script -->
<script type="text/javascript">
var _cdp365Analytics = {             
	 page: {"page_type": "article_detail", "page_category": "<The current article category name>"},      

    items: [{
      type: "article",
      id: "12345", // Article ID
      name: "Review sữa Nan A2 Thụy Sĩ có thực tốt như lời đồn không?", // Article Title
      page_url: window.location.href,
      tags: ["sữa Nan A2", "Sữa Nan A2 Infinipro"],
      tags_string: "sữa Nan A2,Sữa Nan A2 Infinipro"
    }],
    track: [['article', 'view']]        
}
```

