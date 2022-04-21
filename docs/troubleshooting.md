---
title: General Troubleshooting Steps
slug: troubleshooting
cats: Getting Started,Troubleshooting
---


  <p>
    We work hard to proactively avoid conflicts and problems with other themes and plugins, but there will be times when problems crop up.&nbsp;
  </p>
  <p>
    Below is a general guide to troubleshooting problems. If you encounter a problem, follow these steps before reaching out to our support team (it will save time in the long run!)
  </p>
  <h2>
    Step 1: Update your plugins
  </h2>
  <p>
    If you're using outdated versions of WooCommerce, WooCommerce plugins, or CheckoutWC the first course of action is to update these plugins to their latest version.
  </p>
  <p>
    In many cases, the bug you are encountering <a href="https://www.checkoutwc.com/documentation/change-log">may have already been fixed.</a>
  </p>
  <h2>
    Step 2: Make sure you're using a supported checkout field editor (if any)
  </h2>
  <p>
    We support the <a href="https://woocommerce.com/products/woocommerce-checkout-field-editor/" target="_blank">official Checkout Field Editor</a> plugin from WooCommerce.
  </p>
  <p>
    Most other checkout field editor plugins will cause problems - if you're having a an issue, it's always a good idea to try deactivating these types of plugins first.
  </p>
  <h2>
    Step 3: Use a process of elimination to figure out which plugin or theme is causing the issue.
  </h2>
  <p>
    If you don't have a staging site, now is a great time to set one up. (You should have a staging site!)
  </p>
  <p>
    Deactivate all plugins except for:
  </p>
  <ul>
    <li>WooCommerce
    </li>
    <li>CheckoutWC
    </li>
    <li>Payment Gateways
    </li>
    <li>Shipping methods
    </li>
  </ul>
  <p>
    If this fixes the problem, activate the deactivated plugins, one at a time, testing after you activate each one.&nbsp;
  </p>
  <p>
    <strong>You will now know which plugin is causing the issue.</strong> Open a support ticket and send us a zip file (using a Dropbox, Google Drive, or similar link) with a description of how you use the plugin, and any relevant API keys.&nbsp;
  </p>
  <p>
    We'll make every effort to add support (or prevent it from breaking the checkout page).
  </p>
  <h3>
    <strong>If that doesn't fix the problem:</strong>&nbsp;
  </h3>
  <p>
    Try temporarily activating one of the standard WordPress themes.
  </p>
  <p>
    If this fixes the problem, send us a zip file of your theme (and parent theme) using a Dropbox or similar link. We'll figure out what's going on and get you a fix as soon as we can.&nbsp;
  </p>
  <h3>
    <strong>If you are still&nbsp;having problems:</strong>
  </h3>
  <p>
    Try deactivating your payment gateways and shipping methods, one by one, and testing to see which one is causing the problem.&nbsp;
  </p>
  <p>
    You'll have the problem plugin identified quickly using this strategy.&nbsp;
  </p>
  <h3>
    What if I have a lot of plugins?
  </h3>
  <p>
    One way to speed up the process is to use a binary search.&nbsp;
  </p>
  <p>
    Basically, if you have 100 plugins, you would select 50 and deactivate those (obviously skipping the list above).&nbsp;
  </p>
  <p>
    Now test it again. If it fixes the problem, <strong>you know it's in that 50.</strong> If it doesn't fix it, <strong>you know it's in the other 50</strong> and you can reactivate the first 50. Continue dividing the list in half until you get to the offending plugin.&nbsp;
  </p>
  <p>
    It's a process of elimination and it may be much faster than trying to randomly guess which plugin is causing the issue.&nbsp;
  </p>
