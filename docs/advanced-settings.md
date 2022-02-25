---
title: Advanced Settings
slug: advanced-settings
cats: Configuration
---

Advanced has three tabs and let's you configure more advanced features:

Scripts
-------

### Header Scripts and Footer Scripts

Some users will want to add custom tracking scripts and pixels to the checkout page.

You can paste in any tracking scripts into the provided text boxes.

It's also possible to enter your own custom CSS.

NOTE: Scripts and styles must be property wrapped in &lt;script&gt; or &lt;style&gt; tags.

#### Php Snippets

For information about Php Snippets, [please see this document](https://kb.checkoutwc.com/article/94-how-to-add-a-custom-php-snippet).

Integrations
------------

Depending on which plugins you have installed, additional options will appear on the integrations tab:

![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60ae7ed7c1410a601d9ad32e/file-uNRXcrDSSB.png)

### Template Loader

By default, CheckoutWC takes over the whole page when viewing the Checkout, Order Pay, and Thank You pages (depending on what you have configured).

For developers who want more control we have a Template Loader option:

![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60ae7f8b9c887a0dfc553929/file-JMyTeicvD0.png)

If you select WordPress Theme, CheckoutWC will load on the standard \[woocommerce\_checkout\] shortcode.

This option is unsupported - you will most likely need a developer to figure out compatibility issues with your theme.