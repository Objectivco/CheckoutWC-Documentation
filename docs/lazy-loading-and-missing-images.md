---
title: Lazy Loading and Missing Images
slug: lazy-loading-and-missing-images
cats: Troubleshooting
---

 If you see missing images on the checkout page, order pay page, or thank you page **it most likely means that you have enabled your theme's Lazy Loading functionality**.

 **This is because CheckoutWC blocks all JavaScript and CSS files from your theme from being included on the checkout pages.**

 We do this to increase performance reduce compatibility conflicts.

How To Fix Missing Images
-------------------------

 To fix missing images on the checkout page, you should **disable your theme's lazy loading functionality.**

 WordPress Core added [native lazy loading in 5.5](https://make.wordpress.org/core/2020/07/14/lazy-loading-images-in-5-5/). This leverages the loading=lazy attribute supported by most major browser, including Chrome and Firefox.

 This allows browsers to lazy load images without any JavaScript.

 CheckoutWC supports this functionality and most themes properly allow WordPress lazy loading if you disable their lazy loading functionality.

 The only downsides of native lazy loading is that [it isn't currently supported by Safari.](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img#attr-loading) But support is expected soon.

 And as of WordPress 5.7, [support for lazy loading iframes](https://make.wordpress.org/core/2021/02/19/lazy-loading-iframes-in-5-7/) is also enabled!

If You Really Really Need Safari Support
----------------------------------------

 If lazy loading in Safari is crucial for your use case, we recommend [using a lazy load plugin](https://wordpress.org/plugins/rocket-lazy-load/) in favor of using your theme's lazy loading functionality. This will bypass any theme restrictions in CheckoutWC.