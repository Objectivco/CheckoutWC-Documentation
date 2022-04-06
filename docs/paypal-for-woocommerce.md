---
title: Configuring PayPal for WooCommerce with CheckoutWC
slug: paypal-for-woocommerce
cats: 3rd Party Themes and Plugins
---


  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5f74875c52faff00174f4a7c/file-KikTX93dng.png" style="width: 676px;" />
  </p>
  <p>
    Want to add PayPal as an express checkout? We support and recommend <a href="https://www.angelleye.com/product/woocommerce-paypal-plugin/">PayPal for WooCommerce</a> because it provides a fast payment Express button on the checkout page.
  </p>
  <p>
    There is one caveat which is that you can only have one button enabled. This is due to the fact that PayPal renders both buttons in a single iframe.
  </p>
  <p>
    Required: <strong>Enable Smart Buttons</strong> and disable <strong>PayPal Credit</strong>.&nbsp;
  </p>
  <p>
    <img class="alignnone size-full wp-image-1587" src="https://www.checkoutwc.com/wp-content/uploads/2018/11/Screenshot-2018-11-01-14.40.46.png" alt="" width="690" height="230" />
  </p>
  <p>
    Also, you should set the button size to <strong>Medium</strong>:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5c180e812c7d3a31944f35d1/file-bKr3cXJSRS.png" />
  </p>
  <p>
    Set Button Height to 35px so it matches other buttons:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5f7486dbc9e77c001603e1c6/file-UY0iHXYUJn.png" style="width: 679px;" />
  </p>
  <p>
    Set the button shape to rectangle:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5f91d82746e0fb001798fbc9/file-UyIWGp0AvC.png" />
  </p>
  <p>
    You also should make sure that the button is configured to display:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5c3785cf2c7d3a31944fe455/file-G9zrEYK8kn.png" style="width: 677px;" />
  </p>
  <p>
    We also highly recommend you check this option:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60bff1466264f06fc02ff292/file-sI0ueV3yxi.png" />
  </p>
  <p>
    We also recommend you uncheck this option:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5eed10002c7d3a10cba941f6/file-hrQCmoiSoX.png" style="width: 676px;" />
  </p>
  <p>
    This will ensure the button plays well with others. If you are not using other payment buttons and desire to use the credit button, you can override the styling by dropping this into your header scripts setting:
  </p>
  <p>
    <a href="https://gist.github.com/clifgriffin/6e96e784aa9df8c36c30e7d9f6214e48" target="_blank" rel="noopener">Override Checkout for WooCommerce PayPal button styles to allow for more than one smart button.</a>
  </p>
