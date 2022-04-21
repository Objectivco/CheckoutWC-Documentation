---
title: MailChimp for WooCommerce
slug: mailchimp-for-woocommerce
cats: 3rd Party Themes and Plugins
status: published
---


  <p>
    Let's be honest. The MailChimp for WooCommerce plugin leaves a LOT to be desired. Don't believe me? <a href="https://wordpress.org/support/plugin/mailchimp-for-woocommerce/reviews/" target="_blank">Just check the reviews.&nbsp;</a>
  </p>
  <p>
    However assuming you get it working,&nbsp;MailChimp for WooCommerce works with CheckoutWC without any coding required.
  </p>
  <p>
    The only requirement is that you change the default WooCommerce hook that displays the subscribe checkbox. You can do this in the settings under MailChimp &gt; Audience Defaults &gt; Optional Audience Settings:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dfa8d6804286364bc930678/file-sOCtaqqRU9.png" />
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dfa8d8c04286364bc93067b/file-X2OsQonLu6.png" />
  </p>
  <p>
    We recommend this action:
  </p>
  <p>
    cfw_checkout_before_payment_method_tab_nav
  </p>
  <p>
    That places the checkbox right above the complete order button:
  </p>
  <p>
    <img class="alignnone size-full wp-image-949" src="https://www.checkoutwc.com/wp-content/uploads/2018/02/Screenshot-2018-02-15-16.26.57.png" alt="" width="713" height="140" />
  </p>
  <p>
    If you would like to place it under the "Create an account" checkbox, you can use this action:
  </p>
  <p>
    cfw_checkout_after_login
  </p>
  <p>
    <strong>Troubleshooting</strong>
  </p>
  <p>
    One a user subscribes, their account is updated and the checkbox is not shown again. To rule this out, consider testing in an incognito browser window.
  </p>
