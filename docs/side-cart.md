---
title: Side Cart
slug: side-cart
cats: Features
---

 Side Cart is a full cart solution that is designed to replace your cart page with a beautiful and performant side cart. When customers add an item to the cart, the side cart appears from the right.

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/616491b00332cb5b9e9b2a21/file-VML5PgiMUm.gif)

 If you have a **Pro** (10 Sites) or **Agency** (150 Sites) license, you can enable Side Cart in **WP Admin &gt; CheckoutWC &gt; Side Cart.**

Options
-------

 **Enable Floating Cart Button**

 Enables a site wide cart button at the bottom right of the screen:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/61648b69e5648623c88e36ba/file-9t5ONoO9ts.png)

 **Floating Cart Button Right Position**

 The position in pixels that the floating cart button will be rendered from the right side of the screen.

 **Floating Cart Button Bottom Position**

 The position in pixels that the floating cart button will be rendered from the bottom of the screen.

 **Enable AJAX Add to Cart**

 Turns on AJAX add to cart on archive and single product pages.

**Enable Order Bumps**

Turn on to display [Order Bumps](https://kb.checkoutwc.com/article/126-order-bumps) that are set to display below cart items.

**Enable Coupons**

Turn on to allow customers to enter a coupon in the Side Cart.

 **Enable Free Shipping Progress Bar**

 Enable a progress bar that shows the customers how much more they need to add to their cart to qualify for free shipping.

 **Free Shipping Threshold**

 The subtotal amount required for free shipping. If left blank, your shipping methods will be parsed to determine if any of them are of the free shipping type and to determine if they have an amount limit set.

 **Amount Remaining Message**

 What you want to display to the customer letting them know how much they need to add to the cart for free shipping.

 **Free Shipping Message**

 The message displayed to customers to indicate that they have qualified for free shipping.

 **Side Cart Free Shipping Progress Indicator Color**

 The color of the progress bar indicator.

 **Side Cart Free Shipping Progress Background Colo**r

 The color of the progress bar beneath the indicator.

Adding Your Own Cart Link / Button
----------------------------------

 You can easily turn any link or button or HTML element on your website into a cart open button. Simply add this class to the element:

 cfw-side-cart-open-trigger

 For example, you can add the class to menu items:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6169d99012c07c18afddde4f/file-lNGuDOTbAW.png)

 If you don't see **CSS Classes** as an option, click on 'Screen Options' top right and toggle the option for CSS Classes:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6169d9d7efc78d0553e504b0/file-E2xkp0kl0S.png)

 If you can't easily add a class to an element, we have provided another way to tell CheckoutWC about your button. Using this WordPress filter you can specify as many additional buttons as you would like:

<script src="https://gist.github.com/clifgriffin/b3f730210f231bd04ffb199ede6bb913.js" type="text/javascript"></script> The filter receives a string which is a CSS selector that is passed to jQuery. This will make it possible to select any element on the page.

Side Cart Launcher
------------------

 We also have a shortcode for outputting a cart icon + quantity anywhere you would like.

```
[checkoutwc_cart]
```

### Shortcode options:

 **color**

 Example: #222222

 **width:**

 Example: 30px

 **text\_color:**

 Example: #333333

### Full example:

```
[checkoutwc_cart color="#222222" width="30px" text_color="#222222"]
```

### Using in a WordPress menu item

 You can use this simple plugin to add the side cart launcher to a WordPress menu item:

 <https://wordpress.org/plugins/shortcode-in-menus/>