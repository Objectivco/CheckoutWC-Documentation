---
title: How To Add a Custom Field to CheckoutWC
slug: how-to-add-a-custom-field
cats: How To
---

<p>There are a few ways to add a custom field, depending on your exact needs.</p>
<h2>Option 1: Use WooCommerce Checkout Field Editor (Official)</h2>
<p><a href="https://woocommerce.com/products/woocommerce-checkout-field-editor/">WooCommerce Checkout Field Editor</a> is the official checkout field editor plugin.</p>
<p>When active with CheckoutWC, by default only the <strong>Additional Fields</strong> tab is available:</p>
<p>Simply add your fields and save.</p>
<h3>Example configuration:</h3>
<h3><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5d5b1e012c7d3a7920be3bd5/file-QR8DhO6RYE.png" alt="" />What it looks like on checkout:</h3>
<h3><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5d5b1e122c7d3a7920be3bd7/file-0GSSJfuXCy.png" alt="" />Date picker expanded:</h3>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5d5b1e3d2c7d3a7920be3bdd/file-VXE0SA6ZhU.png" alt="" /></p>
<h3>Modifying Billing and Shipping Address Fields with Checkout Field Editor</h3>
<p>Most stores don't need to modify the billing and shipping address fields (and shouldn't!)</p>
<p>But if you would like to use Checkout Field Editor to modify your Billing or Shipping address, here's how you do it.</p>
<h4>Step 1:</h4>
<p>Go to Settings &gt; CheckoutWC &gt; Integrations and check the box next to &quot;Enable Checkout Field Editor address field overrides.&quot;</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dfa99f404286364bc930720/file-I60CIZFfwd.png" alt="" /></p>
<h4>Step 2:</h4>
<p>Modify your addresses under WooCommerce &gt; Checkout Fields.</p>
<h4>Step 3:</h4>
<p>If you are adding a new field to the billing address, you need to add the same field to the shipping address so that the value will be saved to the billing address when the customer selects &quot;Same as shipping address&quot;.</p>
<p>To ensure your fields work properly with this functionality, do the following:</p>
<ol>
<li>Prefix your shipping address fields with <strong>shipping_</strong> or <strong>billing_</strong>. Example: <strong>billing_fax</strong>
</li>
<li>Use the same name for fields that should be synced when 'Same as shipping address' is checked. If you add <strong>shipping_fax</strong>, make sure you name your billing field <strong>billing_fax</strong>.</li>
</ol>
<h2>Option 2: Manually add a custom field to your functions.php file.</h2>
<p>Here's a snippet demonstrating how to add a greeting card field:</p>



<hr />
<p>Checkout Add-ons can also be used for custom fields. These work best if you intend to charge extra for certain options. You can use it without charging, however each field will show up with a $0.00 price line in the totals area.</p>
<p>You will need a license for Checkout Add-ons, which you can get here:</p>
<p><a href="https://woocommerce.com/products/woocommerce-checkout-add-ons/?_ga=2.101477443.314786249.1550432900-1608809788.1474821665">https://woocommerce.com/products/woocommerce-checkout-add-ons/</a></p>
<p>Then just follow their guide to add a custom field:</p>
<p><a href="https://docs.woocommerce.com/document/woocommerce-checkout-add-ons/">https://docs.woocommerce.com/document/woocommerce-checkout-add-ons/</a></p>
