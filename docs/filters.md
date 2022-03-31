---
title: Filters
slug: filters
cats: Developers
---

<h3>apply_filters('cfw_body_classes', array('checkout-wc'))</h3>
<p>Filter classes on &lt;body&gt; tag. Default: checkout-wc</p>
<h3>apply_filters('cfw_get_shipping_checkout_fields', $checkout-&gt;get_checkout_fields( 'shipping' ) );</h3>
<p>Filters an array of shipping address fields.</p>
<h3>apply_filters('cfw_get_billing_checkout_fields', $checkout-&gt;get_checkout_fields( 'billing' ) );</h3>
<p>Filters an array of billing address fields.</p>
<h3>apply_filters('cfw_payment_gateway_field_html_' . $gateway-&gt;id, $field_html);</h3>
<p>Filter the HTML output of each payment gateway.</p>
<h3>apply_filters('cfw_get_template_part_skip_' . $template_part, false)</h3>
<p>Filter whether the given template is loaded by returning true or false (default).</p>
<h3>apply_filters('cfw_show_shipping_tab', true)</h3>
<p>Filter whether the shipping method tab is displayed. (If the cart does not need shipping, the shipping method tab will never be displayed)</p>
<h3>apply_filters('cfw_template_global_params', array());</h3>
<p>Add additional global parameters to the global template parameters object.</p>
<h3>apply_filters('cfw_template_tab_container_el', 'cfw-tab-container');</h3>
<p>Filters the main tab container HTML element ID.</p>
<h3>apply_filters('cfw_template_breadcrumb_id', 'cfw-breadcrumb');</h3>
<p>Filters the breadcrumb HTML element ID.</p>
<h3>apply_filters('cfw_template_customer_info_el', 'cfw-customer-info');</h3>
<p>Filters the customer information tab HTML element ID.</p>
<h3>apply_filters('cfw_template_shipping_method_el', 'cfw-shipping-method');</h3>
<p>Filters the shipping method tab HTML element ID.</p>
<h3>apply_filters('cfw_template_payment_method_el', 'cfw-payment-method');</h3>
<p>Filters the payment method tab HTML element ID.</p>
<h3>apply_filters('cfw_template_cart_el', &quot;cfw-totals-list&quot;);</h3>
<p>Filters the cart container HTML element ID.</p>
<h3>apply_filters('cfw_template_cart_subtotal_el', 'cfw-cart-subtotal');</h3>
<p>Filters the cart subtotal HTML element ID.</p>
<h3>apply_filters('cfw_template_cart_shipping_el', 'cfw-cart-shipping-total');</h3>
<p>Filters the cart shipping HTML element ID.</p>
<h3>apply_filters('cfw_template_cart_taxes_el', 'cfw-cart-taxes');</h3>
<p>Filters the cart taxes HTML element ID.</p>
<h3>apply_filters('cfw_template_cart_total_el','cfw-cart-total');</h3>
<p>Filters the cart total HTML element ID.</p>
<h3>apply_filters('cfw_template_cart_coupons_el', 'cfw-cart-coupons');</h3>
<p>Filters the apply coupon container HTML element ID.</p>
<h3>apply_filters('cfw_template_cart_review_bar_id', 'cfw-cart-details-review-bar');</h3>
<p>Filters the cart review bar HTML element ID.</p>
<h3>apply_filters('cfw_allowed_script_handles', $ignore);</h3>
<p>Filters list of allowed script handles. Scripts handles present in this array will be loaded on the checkout page, even if they are in a 3rd party plugin or theme.</p>
<h3>apply_filters('cfw_allowed_style_handles', $ignore);</h3>
<p>Filters list of allowed style handles. Style handles present in this array will be loaded on the checkout page, even if they are in a 3rd party plugin or theme.</p>
<h3>apply_filters('cfw_customer_information_heading', __( 'Customer information', 'checkout-wc' ) );</h3>
<p>Filter the customer information tab heading.</p>
<h3>apply_filters('cfw_billing_address_heading', esc_html__( 'Billing address', 'checkout-wc' ) );</h3>
<p>Filter the billing address heading.</p>
<h3>apply_filters('cfw_shipping_address_heading', esc_html__( 'Shipping address', 'checkout-wc' ) );</h3>
<p>Filter the shipping address heading.</p>
<h3>apply_filters('cfw_shipping_method_heading', esc_html__( 'Shipping method', 'checkout-wc' ) );</h3>
<p>Filter the shipping method heading.</p>
<h3>apply_filters('cfw_payment_method_heading', esc_html__('Payment method', 'checkout-wc') );</h3>
<p>Filters the payment method heading.</p>
<h3>apply_filters('cfw_no_payment_required_text', esc_html__('Your order is free. No payment is required.', 'checkout-wc') );</h3>
<p>Filters the no payment required text for free orders.</p>
<h3>apply_filters('cfw_link_cart_items', __return_false() )</h3>
<p>Filters whether cart items are linked to their respective products on the checkout page. Default is to not link cart items. Return true to link them.</p>
<h3>apply_filters('cfw_should_load_template_functions', true)</h3>
<p>Turn off checkout template's functions.php file.</p>
<h3>apply_filters('cfw_typescript_compatibility_classes_and_params', [])</h3>
<p>Inject TypeScript classes and parameters from compatibility classes into checkout page.</p>
<h2>apply_filters( 'cfw_check_create_account_by_default', true )</h2>
<p>Controls the default disposition of the create account checkbox. If false, create account will be unchecked by default.</p>
<h2>apply_filters( 'cfw_show_order_summary_link_text', esc_html( 'Show order summary', 'checkout-wc' ) );</h2>
<p>Filter text of 'Show order summary' label on mobile cart.</p>
