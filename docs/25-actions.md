---
title: Actions
slug: actions
cats: Developers
status: published
---


  <h3>
    do_action('cfw_wp_head');
  </h3>
  <p>
    Called immediately before the closing &lt;/head&gt; tag.
  </p>
  <h3>
    do_action('cfw_template_before_load');
  </h3>
  <p>
    Called before the template manager builds the checkout page.&nbsp;
  </p>
  <h3>
    do_action('cfw_template_after_load');
  </h3>
  <p>
    Called after the template manager builds the checkout page.&nbsp;
  </p>
  <h3>
    do_action('cfw_wp_footer_before_scripts');
  </h3>
  <p>
    Called before script functions run in the footer.&nbsp;
  </p>
  <h3>
    do_action('cfw_wp_footer');
  </h3>
  <p>
    Called immediately before the closing &lt;/body&gt; tag.
  </p>
  <h3>
    do_action("cfw_template_load_before_{$template_name}");
  </h3>
  <p>
    Called before template is outputted.
  </p>
  <h3>
    do_action("cfw_template_load_after_{$template_name}");
  </h3>
  <p>
    Called after template is outputted.
  </p>
  <h3>
    do_action('cfw_checkout_before_form');
  </h3>
  <p>
    Called before opening &lt;form&gt; tag.
  </p>
  <h3>
    do_action('cfw_checkout_after_form');
  </h3>
  <p>
    Called after closing &lt;/form&gt; tag.&nbsp;
  </p>
  <h3>
    do_action('cfw_checkout_before_customer_info_tab');
  </h3>
  <p>
    Called at the top of the customer information tab, after the opening &lt;div&gt; tag and before all content.
  </p>
  <h2>
    do_action('cfw_checkout_after_login');
  </h2>
  <p>
    Called at the bottom of the login container.
  </p>
  <h3>
    do_action('cfw_checkout_before_customer_info_address');
  </h3>
  <p>
    Called before the shipping or billing address on the customer information tab.
  </p>
  <h3>
    do_action('cfw_checkout_after_customer_info_address');
  </h3>
  <p>
    Called after the shipping or billing address on the customer information tab.
  </p>
  <h3>
    do_action('cfw_checkout_before_customer_info_tab_nav');
  </h3>
  <p>
    Called before the customer information tab navigation is output.
  </p>
  <h3>
    do_action('cfw_checkout_after_customer_info_tab');
  </h3>
  <p>
    Called after the customer information tab, before the closing &lt;/div&gt; tag.
  </p>
  <h3>
    do_action('cfw_checkout_before_shipping_method_tab');
  </h3>
  <p>
    Called at the top of the shipping method tab, after the opening &lt;div&gt; tag and before all content.
  </p>
  <h3>
    do_action('cfw_checkout_before_shipping_methods');
  </h3>
  <p>
    Called immediately before the shipping methods on the shipping method tab.
  </p>
  <h3>
    do_action('cfw_checkout_after_shipping_methods');
  </h3>
  <p>
    Called immediately after the shipping methods on the shipping method tab.
  </p>
  <h3>
    do_action('cfw_checkout_before_shipping_method_tab_nav');
  </h3>
  <p>
    Called before the shipping method tab navigation is output.&nbsp;
  </p>
  <h3>
    do_action('cfw_checkout_after_shipping_method_tab');
  </h3>
  <p>
    Called after the shipping method tab, before the closing &lt;/div&gt; tag.
  </p>
  <h3>
    do_action('cfw_checkout_before_payment_method_tab');
  </h3>
  <p>
    Called at the top of the payment method tab, after the opening &lt;div&gt; tag and before all content.
  </p>
  <h3>
    do_action('cfw_checkout_before_payment_methods');
  </h3>
  <p>
    Called before the payment methods (gateways) are outputted.&nbsp;
  </p>
  <h3>
    do_action('cfw_checkout_after_payment_methods');
  </h3>
  <p>
    Called after the payment methods (gateways) are outputted.
  </p>
  <h3>
    do_action('cfw_checkout_before_payment_method_terms_checkbox');
  </h3>
  <p>
    Called before the terms and conditions are output on the payment method tab.
  </p>
  <h3>
    do_action('cfw_checkout_before_payment_method_tab_nav');
  </h3>
  <p>
    Called after the terms and conditions are output on the payment method tab.
  </p>
  <h3>
    do_action('cfw_checkout_after_payment_methods_tab');
  </h3>
  <p>
    Called after the payment method tab, before the closing &lt;/div&gt; tag.
  </p>
  <h3>
    do_action( 'cfw_before_footer' );
  </h3>
  <p>
    Called at the top of the footer.
  </p>
  <h3>
    do_action( 'cfw_after_footer' );
  </h3>
  <p>
    Called at the bottom of the footer.
  </p>
  <h3>
    do_action( 'cfw_after_cart_summary_totals' );
  </h3>
  <p>
    Called at the bottom of the cart summary (sidebar on desktop) totals area.&nbsp;
  </p>
  <h3>
    do_action( 'cfw_after_cart_summary' );
  </h3>
  <p>
    Called at the bottom of the cart summary area (sidebar on desktop).
  </p>
