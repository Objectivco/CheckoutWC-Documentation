---
title: Actions
slug: actions
cats: Developers
---

### do\_action('cfw\_wp\_head');

 Called immediately before the closing &lt;/head&gt; tag.

### do\_action('cfw\_template\_before\_load');

 Called before the template manager builds the checkout page.

### do\_action('cfw\_template\_after\_load');

 Called after the template manager builds the checkout page.

### do\_action('cfw\_wp\_footer\_before\_scripts');

 Called before script functions run in the footer.

### do\_action('cfw\_wp\_footer');

 Called immediately before the closing &lt;/body&gt; tag.

### do\_action("cfw\_template\_load\_before\_{$template\_name}");

 Called before template is outputted.

### do\_action("cfw\_template\_load\_after\_{$template\_name}");

 Called after template is outputted.

### do\_action('cfw\_checkout\_before\_form');

 Called before opening &lt;form&gt; tag.

### do\_action('cfw\_checkout\_after\_form');

 Called after closing &lt;/form&gt; tag.

### do\_action('cfw\_checkout\_before\_customer\_info\_tab');

Called at the top of the customer information tab, after the opening &lt;div&gt; tag and before all content.

do\_action('cfw\_checkout\_after\_login');
------------------------------------------

 Called at the bottom of the login container.

### do\_action('cfw\_checkout\_before\_customer\_info\_address');

 Called before the shipping or billing address on the customer information tab.

### do\_action('cfw\_checkout\_after\_customer\_info\_address');

 Called after the shipping or billing address on the customer information tab.

### do\_action('cfw\_checkout\_before\_customer\_info\_tab\_nav');

 Called before the customer information tab navigation is output.

### do\_action('cfw\_checkout\_after\_customer\_info\_tab');

 Called after the customer information tab, before the closing &lt;/div&gt; tag.

### do\_action('cfw\_checkout\_before\_shipping\_method\_tab');

 Called at the top of the shipping method tab, after the opening &lt;div&gt; tag and before all content.

### do\_action('cfw\_checkout\_before\_shipping\_methods');

 Called immediately before the shipping methods on the shipping method tab.

### do\_action('cfw\_checkout\_after\_shipping\_methods');

 Called immediately after the shipping methods on the shipping method tab.

### do\_action('cfw\_checkout\_before\_shipping\_method\_tab\_nav');

 Called before the shipping method tab navigation is output.

### do\_action('cfw\_checkout\_after\_shipping\_method\_tab');

 Called after the shipping method tab, before the closing &lt;/div&gt; tag.

### do\_action('cfw\_checkout\_before\_payment\_method\_tab');

 Called at the top of the payment method tab, after the opening &lt;div&gt; tag and before all content.

### do\_action('cfw\_checkout\_before\_payment\_methods');

 Called before the payment methods (gateways) are outputted.

### do\_action('cfw\_checkout\_after\_payment\_methods');

 Called after the payment methods (gateways) are outputted.

### do\_action('cfw\_checkout\_before\_payment\_method\_terms\_checkbox');

 Called before the terms and conditions are output on the payment method tab.

### do\_action('cfw\_checkout\_before\_payment\_method\_tab\_nav');

 Called after the terms and conditions are output on the payment method tab.

### do\_action('cfw\_checkout\_after\_payment\_methods\_tab');

 Called after the payment method tab, before the closing &lt;/div&gt; tag.

### do\_action( 'cfw\_before\_footer' );

 Called at the top of the footer.

### do\_action( 'cfw\_after\_footer' );

 Called at the bottom of the footer.

### do\_action( 'cfw\_after\_cart\_summary\_totals' );

 Called at the bottom of the cart summary (sidebar on desktop) totals area.

### do\_action( 'cfw\_after\_cart\_summary' );

 Called at the bottom of the cart summary area (sidebar on desktop).
