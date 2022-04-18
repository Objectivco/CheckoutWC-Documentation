---
title: How To Move the Complete Order Button to The Cart Summary Sidebar
slug: how-to-move-the-complete-order-button-to-the-cart-summary-sidebar
cats: How To
---


  <p>
    In some jurisdictions it is legally required to place the Complete Order button beneath the totals. This is necessary to be legally compliant in Germany.&nbsp;
  </p>
  <h2>
    Recommended Method
  </h2>
  <p>
    We now recommend using our Order Review Step feature. More information about configuration is here:
  </p>
  <p>
    <a href="https://cfw.staging.objectiv.co/documentation/how-to-add-order-review-step" target="_blank">How to Add An Order Review Step</a>
  </p>
  <h2>
    OLD METHOD (CheckoutWC 3.x and earlier)
  </h2>
  <script src="https://gist.github.com/clifgriffin/81a131dd49d9cf0075fdb3fe8336cc85.js" type="text/javascript"></script>
  <p>
    This adds the Complete Order button to the bottom of the cart summary sidebar, but it doesn't remove it from its default location. The best way to handle this is with CSS.&nbsp;
  </p>
  <script src="https://gist.github.com/clifgriffin/eadb74b469e5200fe6e3e4992e23d9ba.js" type="text/javascript"></script>
  <h2>
    How to Move the Complete Order Button Below the Order Totals on Mobile
  </h2>
  <p>
    If you want to go a bit further than the default example, you can use this variation of the second block of code:
  </p>
  <script src="https://gist.github.com/clifgriffin/2de8babdb1b87d601ccb1919c36f3aab.js" type="text/javascript"></script>
  <p>
    This is best paired with using this technique:&nbsp;
  </p>
  <p>
    <a href="https://cfw.staging.objectiv.co/documentation/how-to-force-cart-summary-to-stay-expanded-on-mobile" target="_blank">How To Force Cart Summary To Stay Expanded On Mobile</a>
  </p>
  <h2>
    How to Center the Complete Order Button
  </h2>
  <p>
    To center the complete order button, just delete this line from the examples above:
  </p>
  <pre>float: right;
</pre>
