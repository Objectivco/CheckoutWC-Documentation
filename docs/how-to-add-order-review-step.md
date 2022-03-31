---
title: Order Review Step
slug: how-to-add-order-review-step
cats: Features
---

<p>Order Review Step is available to <strong>Plus</strong>, <strong>Pro</strong>, and <strong>Agency</strong> license holders.</p>
<p>Order Review Step adds an additional step to the checkout page after the Payment tab with a summary of the order information and totals.</p>
<p>The Place Order button is beneath this summary, helping with compliance in jurisdictions such as Germany which have stricter rules about how the place order button is oriented.</p>
<p>To enable, go to <strong>WP Admin &gt; CheckoutWC &gt; Checkout</strong> and check the box for 'Enable Order Review Step':</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6009ea672e764327f87c10eb/file-7dgnbZCSL1.png" alt="" /></p>
<p>Once enabled, you'll see an additional step at checkout:</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6009eacbcfe30d219ccda3af/file-5ca9cIsuVF.png" alt="" /></p>
<h2>Problems with Gateways</h2>
<p>A few gateways don't work with our validation trigger. We will list the gateways with known issues here and the known workarounds.</p>
<h3>Stripe (Official)</h3>
<p>If you're using Stripe, you'll need to disable the inline credit card form option:</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6050cd7d3f70ab34d9b9fa6c/file-mtqXE5Na55.png" alt="" /></p>
<p>If this option is enabled and you have a required terms and conditions checkbox, Stripe will throw an error requiring the box to be checked even though it isn't visible on the payment method tab when Order Review Step is active.</p>
<p>Instead, you should disable this option and use the standard CC form.</p>
