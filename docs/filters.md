---
title: Filters
slug: filters
cats: Developers
---

### apply\_filters('cfw\_body\_classes', array('checkout-wc'))

 Filter classes on &lt;body&gt; tag. Default: checkout-wc

### apply\_filters('cfw\_get\_shipping\_checkout\_fields', $checkout-&gt;get\_checkout\_fields( 'shipping' ) );

 Filters an array of shipping address fields.

### apply\_filters('cfw\_get\_billing\_checkout\_fields', $checkout-&gt;get\_checkout\_fields( 'billing' ) );

 Filters an array of billing address fields.

### apply\_filters('cfw\_payment\_gateway\_field\_html\_' . $gateway-&gt;id, $field\_html);

 Filter the HTML output of each payment gateway.

### apply\_filters('cfw\_get\_template\_part\_skip\_' . $template\_part, false)

 Filter whether the given template is loaded by returning true or false (default).

### apply\_filters('cfw\_show\_shipping\_tab', true)

 Filter whether the shipping method tab is displayed. (If the cart does not need shipping, the shipping method tab will never be displayed)

### apply\_filters('cfw\_template\_global\_params', array());

 Add additional global parameters to the global template parameters object.

### apply\_filters('cfw\_template\_tab\_container\_el', 'cfw-tab-container');

 Filters the main tab container HTML element ID.

### apply\_filters('cfw\_template\_breadcrumb\_id', 'cfw-breadcrumb');

 Filters the breadcrumb HTML element ID.

### apply\_filters('cfw\_template\_customer\_info\_el', 'cfw-customer-info');

 Filters the customer information tab HTML element ID.

### apply\_filters('cfw\_template\_shipping\_method\_el', 'cfw-shipping-method');

 Filters the shipping method tab HTML element ID.

### apply\_filters('cfw\_template\_payment\_method\_el', 'cfw-payment-method');

 Filters the payment method tab HTML element ID.

### apply\_filters('cfw\_template\_cart\_el', "cfw-totals-list");

 Filters the cart container HTML element ID.

### apply\_filters('cfw\_template\_cart\_subtotal\_el', 'cfw-cart-subtotal');

 Filters the cart subtotal HTML element ID.

### apply\_filters('cfw\_template\_cart\_shipping\_el', 'cfw-cart-shipping-total');

 Filters the cart shipping HTML element ID.

### apply\_filters('cfw\_template\_cart\_taxes\_el', 'cfw-cart-taxes');

 Filters the cart taxes HTML element ID.

### apply\_filters('cfw\_template\_cart\_total\_el','cfw-cart-total');

 Filters the cart total HTML element ID.

### apply\_filters('cfw\_template\_cart\_coupons\_el', 'cfw-cart-coupons');

 Filters the apply coupon container HTML element ID.

### apply\_filters('cfw\_template\_cart\_review\_bar\_id', 'cfw-cart-details-review-bar');

 Filters the cart review bar HTML element ID.

### apply\_filters('cfw\_allowed\_script\_handles', $ignore);

 Filters list of allowed script handles. Scripts handles present in this array will be loaded on the checkout page, even if they are in a 3rd party plugin or theme.

### apply\_filters('cfw\_allowed\_style\_handles', $ignore);

 Filters list of allowed style handles. Style handles present in this array will be loaded on the checkout page, even if they are in a 3rd party plugin or theme.

### apply\_filters('cfw\_customer\_information\_heading', \_\_( 'Customer information', 'checkout-wc' ) );

 Filter the customer information tab heading.

### apply\_filters('cfw\_billing\_address\_heading', esc\_html\_\_( 'Billing address', 'checkout-wc' ) );

 Filter the billing address heading.

### apply\_filters('cfw\_shipping\_address\_heading', esc\_html\_\_( 'Shipping address', 'checkout-wc' ) );

 Filter the shipping address heading.

### apply\_filters('cfw\_shipping\_method\_heading', esc\_html\_\_( 'Shipping method', 'checkout-wc' ) );

 Filter the shipping method heading.

### apply\_filters('cfw\_payment\_method\_heading', esc\_html\_\_('Payment method', 'checkout-wc') );

 Filters the payment method heading.

### apply\_filters('cfw\_no\_payment\_required\_text', esc\_html\_\_('Your order is free. No payment is required.', 'checkout-wc') );

 Filters the no payment required text for free orders.

### apply\_filters('cfw\_link\_cart\_items', \_\_return\_false() )

 Filters whether cart items are linked to their respective products on the checkout page. Default is to not link cart items. Return true to link them.

### apply\_filters('cfw\_should\_load\_template\_functions', true)

 Turn off checkout template's functions.php file.

### apply\_filters('cfw\_typescript\_compatibility\_classes\_and\_params', \[\])

 Inject TypeScript classes and parameters from compatibility classes into checkout page.

apply\_filters( 'cfw\_check\_create\_account\_by\_default', true )
------------------------------------------------------------------

 Controls the default disposition of the create account checkbox. If false, create account will be unchecked by default.

apply\_filters( 'cfw\_show\_order\_summary\_link\_text', esc\_html( 'Show order summary', 'checkout-wc' ) );
------------------------------------------------------------------------------------------------------------

Filter text of 'Show order summary' label on mobile cart.