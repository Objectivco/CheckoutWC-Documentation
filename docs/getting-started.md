---
title: Getting Started
slug: getting-started
cats: Getting Started
---


  <p>
    Getting started with Checkout for WooCommerce is easy, and for most stores you will be up and running in a few minutes.
  </p>
  <p>
    In this guide, we'll run through some of the basic things you need to think about and test before you go live.
  </p>
  <h2>
    Installation
  </h2>
  <p>
    If you haven't installed CheckoutWC, let's do it. Standard rules apply, and if you need help you can check out our installation guide: <a href="https://cfw.test/documentation/installation">Installation</a>
  </p>
  <h2>
    Activate Your License Key
  </h2>
  <p>
    Before you go any further, you should activate your license key on the <a href="https://cfw.test/documentation/general-settings">General Settings</a> page.&nbsp;
  </p>
  <p>
    A valid and activated license is required in order for the checkout template to display to non-admins and logged out users.&nbsp;
  </p>
  <h2>
    Deactivate Conflicting Plugins
  </h2>
  <p>
    There are a couple of types of plugins that will not work with CheckoutWC by design. These include plugins that manipulate the checkout fields or layout of the checkout page. We do support the official <a href="https://woocommerce.com/products/woocommerce-checkout-field-editor/" target="_blank">Checkout Field Editor</a> plugin, and have <a href="https://cfw.test/documentation/how-to-add-a-custom-field" target="_blank">other options for adding custom fields as well</a>.
  </p>
  <p>
    While we handle a few of these plugins by preventing them from breaking the checkout page, the best solution is to simply disable these plugins. (If you're on the live site, you'll obviously want to time this more carefully so that users don't experience any disruptions)
  </p>
  <h2>
    Pre-flight Testing
  </h2>
  <p>
    After you have installed and activated Checkout for WooCommerce, head over to your store and add a few items to the cart and then proceed to checkout.
  </p>
  <p>
    If everything is working properly, you should have a beautiful fully-functional checkout page.&nbsp;
  </p>
  <p>
    Pay special attention to the payment gateways. Make sure they are displaying properly and the way you would expect. If you're on a staging site, go ahead and put through a test order to confirm everything processes correctly.&nbsp;
  </p>
  <p>
    If you have any problems at this step, check out our troubleshooting guide: <a href="https://cfw.test/documentation/troubleshooting">Troubleshooting</a>
  </p>
  <h2>
    Design
  </h2>
  <p>
    Now that you have confirmed your checkout page is working correctly and activated your license, it's time to add your brand colors.&nbsp;
  </p>
  <p>
    CheckoutWC ships with <a href="https://cfw.test/documentation/appearance-settings">multiple templates</a>, each with their own design options. You can activate each template and then refresh the checkout page to see how they affect the design and layout.
  </p>
  <p>
    Once you have picked a template, you can configure the design in <strong>WP Admin &gt; CheckoutWC &gt; Appearance &gt;&nbsp;Design</strong>. The options on this page are more fully explained in our <a href="https://cfw.test/documentation/appearance-settings">design documentation</a>, but for most stores you'll want to configure these options:
  </p>
  <ul>
    <li>Logo
    </li>
    <li>Primary Colors
    </li>
    <li>Secondary Colors
    </li>
  </ul>
  <p>
    This will allow you to match the branding to your own store.&nbsp;
  </p>
  <h2>
    Tracking Pixels
  </h2>
  <p>
    One common mistake store owners make is to not check their pixel configuration. While most pixel plugins work out of the box, it's a good idea to use your browser add-on (or developer tools) to confirm that the pixel is firing when you expect it to.&nbsp;
  </p>
  <p>
    We have tested many such plugins. You can check out our list of confirmed integrations to verify that your plugin is listed:
  </p>
  <p>
    <a href="https://cfw.test/documentation/integrations">Integrations</a>
  </p>
  <h2>
    <a href="https://cfw.test/documentation/integrations"></a>Testing
  </h2>
  <p>
    Your checkout page is crucial to your business. It's imperative that you thoroughly test your store before <a href="https://cfw.test/documentation/general-settings">enabling it for all users</a>.
  </p>
  <h4>
    <strong>You should also test before updating.</strong>&nbsp;
  </h4>
  <p>
    While our automated End-to-End testing catches many problems, it will never be 100% and it can never test your store.&nbsp;
  </p>
  <p>
    Each release has a change log that will give you a sense of how extensive that update is. We generally try to follow the rules of semantic versioning. If you see a major release (4.x -&gt; 5.x), you can assume new functionality and (potentially) breaking changes.&nbsp;
  </p>
  <p>
    If you see a minor release (5.0.0 -&gt; 5.1.0) you can expect larger scale changes that could-be, but probably aren't breaking.&nbsp;
  </p>
  <p>
    For patch level changes (5.1.1 -&gt; 5.1.2), we would not expect any breaking changes. These are usually bug fixes to address specific customer support requests.&nbsp;
  </p>
  <p>
    We recommend that every merchant have a staging/testing site that they use to verify that orders can be submitted successfully before updating their live site. If you need an extra license key for a staging site, contact support and we'll be happy to add one for you. &nbsp;
  </p>
  <h4>
    Keeping your store running is your responsibility.
  </h4>
  <p>
    We make every effort to test each release, but your store is unique what works for 1000 stores might not work for your 1 store. <strong>You should always test before updating a live site that is taking orders.</strong>
  </p>
  <h2>
    Go Live
  </h2>
  <p>
    Once you have configured the checkout page to your liking, head over to General Settings and activate CheckoutWC for the world. ðŸš€
  </p>
  <h2>
    Getting Support
  </h2>
  <p>
    We pride ourselves on offering great support. If you encounter any problems, head over to <strong>WP Admin &gt; CheckoutWC &gt; Support</strong>&nbsp;and drop us a note.&nbsp;
  </p>
  <p>
    We strive to be very responsive to support tickets, and we'll get you a solution as fast as we can.&nbsp;
  </p>
  <p>
    Thanks again for choosing CheckoutWC!
  </p>
