---
title: Thank You Page
slug: how-to-enable-and-configure-the-thank-you-page
cats: Features
---

 The Thank You page feature replaces the order received page with a beautiful design that closely resembles the checkout page. This same template is used for viewing orders from My Account. It looks like this:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0c2742c7d3a7e9ae38058/file-oTIO1bLH1L.png)

 There are a number of configuration steps but most are optional and it will work pretty basically out of the box.

 Please note: This premium feature is available to **Plus, Pro,** and **Agency** license holders.

Step 1: Enable Thank You Page
-----------------------------

 Go to **WP Admin** &gt; **CheckoutWC** &gt; **Thank You** and toggle the checkbox next to 'Enable support for thank you page.'

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0889604286364bc915295/file-2h65VIXadr.gif)

Step 2: Configure Order Statuses (Optional)
-------------------------------------------

 When you enable the Thank You Page in Step 1, you'll notice a new option appear: **Order Statuses**

 This allows you to define which statuses show up in the status row:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0890a2c7d3a7e9ae37e12/file-ipoHVJWthV.png)

 To select the order statuses you want to show, pick them from the list and click **Save Changes:**

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc08a9e2c7d3a7e9ae37e1f/file-J4udliUx1G.gif)

### Step 2a: Sorting Order Statuses 

 The sort order of these statuses depends on two things:

1. If you are using [WooCommerce Order Status Manager](https://woocommerce.com/products/woocommerce-order-status-manager/), the order is determined by the order you configure in the status settings. The Post Attributes setting allows you to define an order. These are ordered from least (0 0) to greatest (a very large number)![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0894f2c7d3a7e9ae37e15/file-D5uSSYR5r7.png)
2. If you are NOT using WooCommerce Order Status Manager, you'll have to add some custom code to re-order the statuses into the order you prefer. This is beyond the scope of support, but the filter you should use is: **wc\_order\_statuses**

 It is not always necessary to resort the statuses, the order they appear in the dropdown is the order they will be listed on the checkout page.

Step 3: Configure Map Embed (Optional)
--------------------------------------

 The thank you page includes an optional map embed that looks like this:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc08aee2c7d3a7e9ae37e24/file-4PnRvnPJjx.png)

 To enable the map, you need to toggle the setting and provide a **Google API Key**.

 To enable the setting, toggle 'Enable map embed' under Settings &gt; CheckoutWC &gt; General:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc08b2904286364bc9152ab/file-NG1Q5qVz6Q.png)

 The Google API Key is shared with the [Address Autocomplete](https://kb.checkoutwc.com/article/72-how-to-enable-address-autocomplete) setting. If you already have Address Autocomplete enabled, this will save a bit of time.

 Configuring Google API Keys can be a bit tedious, to help guide you in the process we have created a separate doc: [How To Get and Configure Your Google API Key](https://kb.checkoutwc.com/article/86-how-to-get-and-configure-your-google-api-key)

Step 4: Configure Order Status Icons (Optional)
-----------------------------------------------

 The order status row allows you to include an icon for each order status as seen here:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0890a2c7d3a7e9ae37e12/file-ipoHVJWthV.png)

 If you're using WooCommerce Order Status Manager, you can easily setup your icons. Go to WooCommerce &gt; Settings &gt; Order Statuses and click on the status you want to change. Then select your icon like this:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc09f452c7d3a7e9ae37f2f/file-jjK1iXc94g.gif)

 NOTE: Due to the complexity of supporting other icon packages, we currently only support FontAwesome. The icon collection we load is FontAwesome 4.70 which you can browse here: <https://fontawesome.com/v4.7.0/>

### How to use icons if you don't have WooCommerce Order Status Manager

 If you don't have WooCommerce Order Status Manager, you can still configure icons but it will take a little bit of coding. The icon library you can use is [FontAwesome 4.7.0](https://fontawesome.com/v4.7.0/). You just need to lookup the desired icon and then provide the icon classes. Here's a quick example that shows you how to use the check mark icon for the Pending status:

<script src="https://gist.github.com/clifgriffin/2e858e85b8a4aceddd61195dada5c1d8.js" type="text/javascript"></script> You'll notice you have to provide both classes from FontAwesome, which you can see highlighted here:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0a35504286364bc9153db/file-dunMeEJHeg.png)

### Using a different font library

 Because the above filter just returns a class, you can theoretically use any icon library that uses an *I* element with specific classes. You would just need to setup the classes using the above filter and then add the font library to **WP Admin &gt; CheckoutWC &gt; Appearance &gt; Design &gt; Custom CSS**.