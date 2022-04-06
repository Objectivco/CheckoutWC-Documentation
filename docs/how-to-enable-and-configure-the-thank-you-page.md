---
title: Thank You Page
slug: how-to-enable-and-configure-the-thank-you-page
cats: Features
---


  <p>
    The Thank You page feature replaces the order received page with a beautiful design that closely resembles the checkout page. This same template is used for viewing orders from My Account. It looks like this:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0c2742c7d3a7e9ae38058/file-oTIO1bLH1L.png" />
  </p>
  <p>
    There are a number of configuration steps but most are optional and it will work pretty basically out of the box.
  </p>
  <p>
    Please note: This premium feature is available to &nbsp;<strong>Plus, Pro,&nbsp;</strong>and&nbsp;<strong>Agency</strong>&nbsp;license holders.
  </p>
  <h2>
    Step 1: Enable Thank You Page
  </h2>
  <p>
    Go to <strong>WP Admin</strong> &gt; <strong>CheckoutWC</strong> &gt; <strong>Thank You</strong>&nbsp;and toggle the checkbox next to 'Enable support for thank you page.'
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0889604286364bc915295/file-2h65VIXadr.gif" />
  </p>
  <h2>
    Step 2: Configure Order Statuses (Optional)
  </h2>
  <p>
    When you enable the Thank You Page in Step 1, you'll notice a new option appear: <strong>Order Statuses</strong>
  </p>
  <p>
    This allows you to define which statuses show up in the status row:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0890a2c7d3a7e9ae37e12/file-ipoHVJWthV.png" />
  </p>
  <p>
    To select the order statuses you want to show, pick them from the list and click <strong>Save Changes:</strong>
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc08a9e2c7d3a7e9ae37e1f/file-J4udliUx1G.gif" />
  </p>
  <h3>
    Step 2a: Sorting Order Statuses&nbsp;
  </h3>
  <p>
    The sort order of these statuses depends on two things:
  </p>
  <ol>
    <li>If you are using <a href="https://woocommerce.com/products/woocommerce-order-status-manager/" target="_blank">WooCommerce Order Status Manager</a>, the order is determined by the order you configure in the status settings. The Post Attributes setting allows you to define an order. These are ordered from least (0 0) to greatest (a very large number)<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0894f2c7d3a7e9ae37e15/file-D5uSSYR5r7.png" />
    </li>
    <li>If you are NOT using WooCommerce Order Status Manager, you'll have to add some custom code to re-order the statuses into the order you prefer. This is beyond the scope of support, but the filter you should use is:&nbsp;<strong>wc_order_statuses</strong>&nbsp;
    </li>
  </ol>
  <p>
    It is not always&nbsp;necessary to resort the statuses, the order they appear in the dropdown is the order they will be listed on the checkout page.
  </p>
  <h2>
    Step 3: Configure Map Embed (Optional)
  </h2>
  <p>
    The thank you page includes an optional map embed that looks like this:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc08aee2c7d3a7e9ae37e24/file-4PnRvnPJjx.png" />
  </p>
  <p>
    To enable the map, you need to toggle the setting and provide a <strong>Google API Key</strong>.
  </p>
  <p>
    To enable the setting, toggle 'Enable map embed' under Settings &gt; CheckoutWC &gt; General:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc08b2904286364bc9152ab/file-NG1Q5qVz6Q.png" />
  </p>
  <p>
    The Google API Key is shared with the <a href="https://cfw.test/documentation/how-to-enable-address-autocomplete" target="_blank">Address Autocomplete</a> setting. If you already have Address Autocomplete enabled, this will save a bit of time.&nbsp;
  </p>
  <p>
    Configuring Google API Keys can be a bit tedious, to help guide you in the process we have created a separate doc: <a href="https://cfw.test/documentation/how-to-get-and-configure-your-google-api-key" target="_blank">How To Get and Configure Your Google API Key</a>
  </p>
  <h2>
    Step 4: Configure Order Status Icons (Optional)
  </h2>
  <p>
    The order status row allows you to &nbsp;include an icon for each order status as seen here:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0890a2c7d3a7e9ae37e12/file-ipoHVJWthV.png" />
  </p>
  <p>
    If you're using WooCommerce Order Status Manager, you can easily setup your icons. Go to WooCommerce &gt; Settings &gt; Order Statuses and click on the status you want to change. Then select your icon like this:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc09f452c7d3a7e9ae37f2f/file-jjK1iXc94g.gif" />
  </p>
  <p>
    NOTE: Due to the complexity of supporting other icon packages, we currently only support FontAwesome. The icon collection we load is FontAwesome 4.70 which you can browse here: <a href="https://fontawesome.com/v4.7.0/" target="_blank">https://fontawesome.com/v4.7.0/</a>
  </p>
  <h3>
    How to use icons if you don't have WooCommerce Order Status Manager
  </h3>
  <p>
    If you don't have WooCommerce Order Status Manager, you can still configure icons but it will take a little bit of coding. &nbsp;The icon library you can use is <a href="https://fontawesome.com/v4.7.0/" target="_blank">FontAwesome 4.7.0</a>. You just need to lookup the desired icon and then provide the icon classes. Here's a quick example that shows you how to use the check mark icon for the Pending status:
  </p>
  <script src="https://gist.github.com/clifgriffin/2e858e85b8a4aceddd61195dada5c1d8.js" type="text/javascript"></script>
  <p>
    You'll notice you have to provide both classes from FontAwesome, which you can see highlighted here:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0a35504286364bc9153db/file-dunMeEJHeg.png" />
  </p>
  <h3>
    Using a different font library
  </h3>
  <p>
    Because the above filter just returns a class, you can theoretically use any icon library that uses an&nbsp;<em>I</em>&nbsp;element with specific classes. You would just need to setup the classes using the above filter and then add the font library to <strong>WP Admin &gt; CheckoutWC &gt; Appearance &gt; Design &gt; Custom CSS</strong>.&nbsp;
  </p>
