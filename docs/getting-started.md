---
title: Getting Started
slug: getting-started
cats: Getting Started
---

 Getting started with Checkout for WooCommerce is easy, and for most stores you will be up and running in a few minutes.

 In this guide, we'll run through some of the basic things you need to think about and test before you go live.

Installation
------------

 If you haven't installed CheckoutWC, let's do it. Standard rules apply, and if you need help you can check out our installation guide: [Installation](https://kb.checkoutwc.com/article/4-installation)

Activate Your License Key
-------------------------

 Before you go any further, you should activate your license key on the [General Settings](https://kb.checkoutwc.com/article/19-general-settings) page.

 A valid and activated license is required in order for the checkout template to display to non-admins and logged out users.

Deactivate Conflicting Plugins
------------------------------

 There are a couple of types of plugins that will not work with CheckoutWC by design. These include plugins that manipulate the checkout fields or layout of the checkout page. We do support the official [Checkout Field Editor](https://woocommerce.com/products/woocommerce-checkout-field-editor/) plugin, and have [other options for adding custom fields as well](https://kb.checkoutwc.com/article/49-how-to-add-a-custom-field).

 While we handle a few of these plugins by preventing them from breaking the checkout page, the best solution is to simply disable these plugins. (If you're on the live site, you'll obviously want to time this more carefully so that users don't experience any disruptions)

Pre-flight Testing
------------------

 After you have installed and activated Checkout for WooCommerce, head over to your store and add a few items to the cart and then proceed to checkout.

 If everything is working properly, you should have a beautiful fully-functional checkout page.

 Pay special attention to the payment gateways. Make sure they are displaying properly and the way you would expect. If you're on a staging site, go ahead and put through a test order to confirm everything processes correctly.

 If you have any problems at this step, check out our troubleshooting guide: [Troubleshooting](https://kb.checkoutwc.com/article/36-troubleshooting)

Design
------

 Now that you have confirmed your checkout page is working correctly and activated your license, it's time to add your brand colors.

 CheckoutWC ships with [multiple templates](https://kb.checkoutwc.com/article/130-appearance-settings), each with their own design options. You can activate each template and then refresh the checkout page to see how they affect the design and layout.

 Once you have picked a template, you can configure the design in **WP Admin &gt; CheckoutWC &gt; Appearance &gt; Design**. The options on this page are more fully explained in our [design documentation](https://kb.checkoutwc.com/article/130-appearance-settings), but for most stores you'll want to configure these options:

- Logo
- Primary Colors
- Secondary Colors

 This will allow you to match the branding to your own store.

Tracking Pixels
---------------

 One common mistake store owners make is to not check their pixel configuration. While most pixel plugins work out of the box, it's a good idea to use your browser add-on (or developer tools) to confirm that the pixel is firing when you expect it to.

 We have tested many such plugins. You can check out our list of confirmed integrations to verify that your plugin is listed:

 [Integrations](https://kb.checkoutwc.com/article/6-integrations)

[](https://kb.checkoutwc.com/article/6-integrations)Testing
-----------------------------------------------------------

 Your checkout page is crucial to your business. It's imperative that you thoroughly test your store before [enabling it for all users](https://kb.checkoutwc.com/article/19-general-settings).

####  **You should also test before updating.**

While our automated End-to-End testing catches many problems, it will never be 100% and it can never test your store.

 Each release has a change log that will give you a sense of how extensive that update is. We generally try to follow the rules of semantic versioning. If you see a major release (4.x -&gt; 5.x), you can assume new functionality and (potentially) breaking changes.

If you see a minor release (5.0.0 -&gt; 5.1.0) you can expect larger scale changes that could-be, but probably aren't breaking.

For patch level changes (5.1.1 -&gt; 5.1.2), we would not expect any breaking changes. These are usually bug fixes to address specific customer support requests.

 We recommend that every merchant have a staging/testing site that they use to verify that orders can be submitted successfully before updating their live site. If you need an extra license key for a staging site, contact support and we'll be happy to add one for you.

#### Keeping your store running is your responsibility.

We make every effort to test each release, but your store is unique what works for 1000 stores might not work for your 1 store. **You should always test before updating a live site that is taking orders.**

Go Live
-------

 Once you have configured the checkout page to your liking, head over to General Settings and activate CheckoutWC for the world. 🚀

Getting Support
---------------

 We pride ourselves on offering great support. If you encounter any problems, head over to **WP Admin &gt; CheckoutWC &gt; Support** and drop us a note.

 We strive to be very responsive to support tickets, and we'll get you a solution as fast as we can.

 Thanks again for choosing CheckoutWC!