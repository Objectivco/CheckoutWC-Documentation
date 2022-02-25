---
title: How To Customize Fonts
slug: how-to-modify-fonts
cats: How To
---

 Checkout for WooCommerce uses the system font stack by default.

 This has the[ advantage of be lightning fast as well as well as matching the user's OS defaults](https://css-tricks.com/snippets/css/system-font-stack/).

Using Google Fonts
------------------

To change your fonts, go to **Settings** &gt; **CheckoutWC** &gt; **Design** and change the the Body Font and Heading Font settings:

![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e90c4b22c7d3a7e9aeac48b/file-tmOO1dt37a.png)

Then save your settings and you're good to go.

If your font list isn't loading.
--------------------------------

Occasionally, our fetch to Google may return an error which gets cached as a transient. To fix this, try deleting all of your transients.

With WP CLI you can use this:

wp transient delete --all

If you don't have access to WP CLI, you can use a plugin like this:

<https://wordpress.org/plugins/transients-manager/>

Using custom fonts.
-------------------

If you can't find the font you need with Google Fonts, you can add a custom font. This will require custom coding.

You can insert your style tags into **Settings** &gt; **CheckoutWC** &gt; **General** &gt; **Header Scripts**.

We can't really help with this part, but if you run into a snag you're welcome to contact support and we'll try to point you in the right direction.