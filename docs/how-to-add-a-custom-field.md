---
title: How To Add a Custom Field to CheckoutWC
slug: how-to-add-a-custom-field
cats: How To
---

 There are a few ways to add a custom field, depending on your exact needs.

Option 1: Use WooCommerce Checkout Field Editor (Official)
----------------------------------------------------------

 [WooCommerce Checkout Field Editor](https://woocommerce.com/products/woocommerce-checkout-field-editor/) is the official checkout field editor plugin.

 When active with CheckoutWC, by default only the **Additional Fields** tab is available:

 Simply add your fields and save.

### Example configuration:

### ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5d5b1e012c7d3a7920be3bd5/file-QR8DhO6RYE.png)What it looks like on checkout:

### ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5d5b1e122c7d3a7920be3bd7/file-0GSSJfuXCy.png)Date picker expanded:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5d5b1e3d2c7d3a7920be3bdd/file-VXE0SA6ZhU.png)

### Modifying Billing and Shipping Address Fields with Checkout Field Editor

 Most stores don't need to modify the billing and shipping address fields (and shouldn't!)

 But if you would like to use Checkout Field Editor to modify your Billing or Shipping address, here's how you do it.

#### Step 1:

 Go to Settings &gt; CheckoutWC &gt; Integrations and check the box next to "Enable Checkout Field Editor address field overrides."

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dfa99f404286364bc930720/file-I60CIZFfwd.png)

#### Step 2:

 Modify your addresses under WooCommerce &gt; Checkout Fields.

#### Step 3:

 If you are adding a new field to the billing address, you need to add the same field to the shipping address so that the value will be saved to the billing address when the customer selects "Same as shipping address".

 To ensure your fields work properly with this functionality, do the following:

1. Prefix your shipping address fields with **shipping\_** or **billing\_**. Example: **billing\_fax**
2. Use the same name for fields that should be synced when 'Same as shipping address' is checked. If you add **shipping\_fax**, make sure you name your billing field **billing\_fax**.

Option 2: Manually add a custom field to your functions.php file.
-----------------------------------------------------------------

 Here's a snippet demonstrating how to add a greeting card field:

<script src="https://gist.github.com/clifgriffin/e4666d5fb200514bcd0e68b2a06e8c7b.js" type="text/javascript"></script> Here's how to add a signature required checkbox:

<script src="https://gist.github.com/clifgriffin/e36f16a1e237ec2205a890cc612c420c.js" type="text/javascript"></script> Here's an example of a required checkbox:

<script src="https://gist.github.com/clifgriffin/63394170dd7ca8e3d0c1d4393a1d69cd.js" type="text/javascript"></script>Option 3: Use Checkout Add-ons
------------------------------

 Checkout Add-ons can also be used for custom fields. These work best if you intend to charge extra for certain options. You can use it without charging, however each field will show up with a $0.00 price line in the totals area.

 You will need a license for Checkout Add-ons, which you can get here:

 [https://woocommerce.com/products/woocommerce-checkout-add-ons/](https://woocommerce.com/products/woocommerce-checkout-add-ons/?_ga=2.101477443.314786249.1550432900-1608809788.1474821665)

 Then just follow their guide to add a custom field:

 <https://docs.woocommerce.com/document/woocommerce-checkout-add-ons/>