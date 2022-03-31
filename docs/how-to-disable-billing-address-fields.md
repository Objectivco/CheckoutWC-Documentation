---
title: How to Remove / Disable Billing Address Fields
slug: how-to-disable-billing-address-fields
cats: How To
---

<p>It is sometimes desirable to remove or otherwise disable billing address fields during checkout. How you do this depends on the type of store you're running and what you're trying to achieve.</p>
<h2>Scenario 1: Stores with shipped products.</h2>
<p>If you sell shipped products and you don't need customer to enter a separate billing address, you can use the built in WooCommerce address features.</p>
<h4>1) In WordPress admin, go to WooCommerce &gt; Settings</h4>
<h4>2) Click the Shipping tab</h4>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e19f4d12c7d3a7e9ae61194/file-O3skaW8Q5D.png" alt="" /></p>
<h4>3) Click 'Shipping options'</h4>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e19f4e32c7d3a7e9ae61195/file-GjbLjZfHUS.png" alt="" /></p>
<h4>4) Select 'Force shipping to customer billing address' for 'Shipping destination' and save.</h4>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e19f50f04286364bc93c24d/file-2c85P2TE4s.png" alt="" /></p>
<h4>5) (Optional) Change the address heading.</h4>
<p>By default, the heading for the address fields will be 'Billing and Shipping address'. You can override this with this snippet:</p>

<hr />
<p>If you want to remove billing address fields, you'll need to use the following code snippet. You can remove any billing address lines that are not required by your store in two steps:</p>
<p><strong>NOTE: If you have the country field enabled, you must also enable to State field or errors will occur. WooCommerce's country / state handlers get messed up when only one is present.</strong></p>
<ol>
<li>
<p>Remove the field from the checkout page.</p>
</li>
<li>
<p>Tell WooCommerce the field is not required.</p>
</li>
</ol>
<p>This snippet accomplishes both purposes:</p>

