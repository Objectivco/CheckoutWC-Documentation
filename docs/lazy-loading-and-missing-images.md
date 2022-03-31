---
title: Lazy Loading and Missing Images
slug: lazy-loading-and-missing-images
cats: Troubleshooting
---

<p>If you see missing images on the checkout page, order pay page, or thank you page <strong>it most likely means that you have enabled your theme's Lazy Loading functionality</strong>.</p>
<p><strong>This is because CheckoutWC blocks all JavaScript and CSS files from your theme from being included on the checkout pages.</strong></p>
<p>We do this to increase performance reduce compatibility conflicts.</p>
<h2>How To Fix Missing Images</h2>
<p>To fix missing images on the checkout page, you should <strong>disable your theme's lazy loading functionality.</strong></p>
<p>WordPress Core added <a href="https://make.wordpress.org/core/2020/07/14/lazy-loading-images-in-5-5/">native lazy loading in 5.5</a>. This leverages the loading=lazy attribute supported by most major browser, including Chrome and Firefox.</p>
<p>This allows browsers to lazy load images without any JavaScript.</p>
<p>CheckoutWC supports this functionality and most themes properly allow WordPress lazy loading if you disable their lazy loading functionality.</p>
<p>The only downsides of native lazy loading is that <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img#attr-loading">it isn't currently supported by Safari.</a> But support is expected soon.</p>
<p>And as of WordPress 5.7, <a href="https://make.wordpress.org/core/2021/02/19/lazy-loading-iframes-in-5-7/">support for lazy loading iframes</a> is also enabled!</p>
<h2>If You Really Really Need Safari Support</h2>
<p>If lazy loading in Safari is crucial for your use case, we recommend <a href="https://wordpress.org/plugins/rocket-lazy-load/">using a lazy load plugin</a> in favor of using your theme's lazy loading functionality. This will bypass any theme restrictions in CheckoutWC.</p>
