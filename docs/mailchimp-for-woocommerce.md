---
title: MailChimp for WooCommerce
slug: mailchimp-for-woocommerce
cats: 3rd Party Themes and Plugins
---

 Let's be honest. The MailChimp for WooCommerce plugin leaves a LOT to be desired. Don't believe me? [Just check the reviews. ](https://wordpress.org/support/plugin/mailchimp-for-woocommerce/reviews/)

 However assuming you get it working, MailChimp for WooCommerce works with CheckoutWC without any coding required.

 The only requirement is that you change the default WooCommerce hook that displays the subscribe checkbox. You can do this in the settings under MailChimp &gt; Audience Defaults &gt; Optional Audience Settings:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dfa8d6804286364bc930678/file-sOCtaqqRU9.png)

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dfa8d8c04286364bc93067b/file-X2OsQonLu6.png)

 We recommend this action:

 cfw\_checkout\_before\_payment\_method\_tab\_nav

 That places the checkbox right above the complete order button:

 ![](https://www.checkoutwc.com/wp-content/uploads/2018/02/Screenshot-2018-02-15-16.26.57.png)

 If you would like to place it under the "Create an account" checkbox, you can use this action:

 cfw\_checkout\_after\_login

**Troubleshooting**

One a user subscribes, their account is updated and the checkbox is not shown again. To rule this out, consider testing in an incognito browser window.