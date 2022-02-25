---
title: How to Remove / Disable Billing Address Fields
slug: how-to-disable-billing-address-fields
cats: How To
---

 It is sometimes desirable to remove or otherwise disable billing address fields during checkout. How you do this depends on the type of store you're running and what you're trying to achieve.

Scenario 1: Stores with shipped products.
-----------------------------------------

 If you sell shipped products and you don't need customer to enter a separate billing address, you can use the built in WooCommerce address features.

#### 1) In WordPress admin, go to WooCommerce &gt; Settings

#### 2) Click the Shipping tab

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e19f4d12c7d3a7e9ae61194/file-O3skaW8Q5D.png)

#### 3) Click 'Shipping options'

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e19f4e32c7d3a7e9ae61195/file-GjbLjZfHUS.png)

#### 4) Select 'Force shipping to customer billing address' for 'Shipping destination' and save.

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e19f50f04286364bc93c24d/file-2c85P2TE4s.png)

#### 5) (Optional) Change the address heading. 

 By default, the heading for the address fields will be 'Billing and Shipping address'. You can override this with this snippet:

<script src="https://gist.github.com/clifgriffin/3f973630c5b91b30ba56fe7c8f338b94.js" type="text/javascript"></script>Scenario 2: Digital stores that don't need a full billing address
-----------------------------------------------------------------

 If you want to remove billing address fields, you'll need to use the following code snippet. You can remove any billing address lines that are not required by your store in two steps:

**NOTE: If you have the country field enabled, you must also enable to State field or errors will occur. WooCommerce's country / state handlers get messed up when only one is present.**

 1) Remove the field from the checkout page.

 2) Tell WooCommerce the field is not required.

 This snippet accomplishes both purposes:

<script src="https://gist.github.com/clifgriffin/818a5ac1e8809e0ad8a4cf079e2590d4.js" type="text/javascript"></script>