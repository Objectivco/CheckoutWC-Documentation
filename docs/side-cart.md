---
title: Side Cart
slug: side-cart
cats: Features
---

<p>Side Cart is a full cart solution that is designed to replace your cart page with a beautiful and performant side cart. When customers add an item to the cart, the side cart appears from the right.</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/616491b00332cb5b9e9b2a21/file-VML5PgiMUm.gif" alt="" /></p>
<p>If you have a <strong>Pro</strong> (10 Sites) or <strong>Agency</strong> (150 Sites) license, you can enable Side Cart in <strong>WP Admin &gt; CheckoutWC &gt; Side Cart.</strong></p>
<h2>Options</h2>
<p><strong>Enable Floating Cart Button</strong></p>
<p>Enables a site wide cart button at the bottom right of the screen:</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/61648b69e5648623c88e36ba/file-9t5ONoO9ts.png" alt="" /></p>
<p><strong>Floating Cart Button Right Position</strong></p>
<p>The position in pixels that the floating cart button will be rendered from the right side of the screen.</p>
<p><strong>Floating Cart Button Bottom Position</strong></p>
<p>The position in pixels that the floating cart button will be rendered from the bottom of the screen.</p>
<p><strong>Enable AJAX Add to Cart</strong></p>
<p>Turns on AJAX add to cart on archive and single product pages.</p>
<p><strong>Enable Order Bumps</strong></p>
<p>Turn on to display <a href="https://kb.checkoutwc.com/article/126-order-bumps">Order Bumps</a> that are set to display below cart items.</p>
<p><strong>Enable Coupons</strong></p>
<p>Turn on to allow customers to enter a coupon in the Side Cart.</p>
<p><strong>Enable Free Shipping Progress Bar</strong></p>
<p>Enable a progress bar that shows the customers how much more they need to add to their cart to qualify for free shipping.</p>
<p><strong>Free Shipping Threshold</strong></p>
<p>The subtotal amount required for free shipping. If left blank, your shipping methods will be parsed to determine if any of them are of the free shipping type and to determine if they have an amount limit set.</p>
<p><strong>Amount Remaining Message</strong></p>
<p>What you want to display to the customer letting them know how much they need to add to the cart for free shipping.</p>
<p><strong>Free Shipping Message</strong></p>
<p>The message displayed to customers to indicate that they have qualified for free shipping.</p>
<p><strong>Side Cart Free Shipping Progress Indicator Color</strong></p>
<p>The color of the progress bar indicator.</p>
<p><strong>Side Cart Free Shipping Progress Background Colo</strong>r</p>
<p>The color of the progress bar beneath the indicator.</p>
<h2>Adding Your Own Cart Link / Button</h2>
<p>You can easily turn any link or button or HTML element on your website into a cart open button. Simply add this class to the element:</p>
<p>cfw-side-cart-open-trigger</p>
<p>For example, you can add the class to menu items:</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6169d99012c07c18afddde4f/file-lNGuDOTbAW.png" alt="" /></p>
<p>If you don't see <strong>CSS Classes</strong> as an option, click on 'Screen Options' top right and toggle the option for CSS Classes:</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6169d9d7efc78d0553e504b0/file-E2xkp0kl0S.png" alt="" /></p>
<p>If you can't easily add a class to an element, we have provided another way to tell CheckoutWC about your button. Using this WordPress filter you can specify as many additional buttons as you would like:</p>

<h2>Side Cart Launcher</h2>
<p>We also have a shortcode for outputting a cart icon + quantity anywhere you would like.</p>
<pre><code>[checkoutwc_cart]
</code></pre>
<h3>Shortcode options:</h3>
<p><strong>color</strong></p>
<p>Example: #222222</p>
<p><strong>width:</strong></p>
<p>Example: 30px</p>
<p><strong>text_color:</strong></p>
<p>Example: #333333</p>
<h3>Full example:</h3>
<pre><code>[checkoutwc_cart color=&quot;#222222&quot; width=&quot;30px&quot; text_color=&quot;#222222&quot;]
</code></pre>
<h3>Using in a WordPress menu item</h3>
<p>You can use this simple plugin to add the side cart launcher to a WordPress menu item:</p>
<p><a href="https://wordpress.org/plugins/shortcode-in-menus/">https://wordpress.org/plugins/shortcode-in-menus/</a></p>
