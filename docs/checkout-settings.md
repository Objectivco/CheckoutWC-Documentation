---
title: Checkout Settings
slug: checkout-settings
cats: Configuration
---

 Order Notes
------------

 Determine whether the order notes appear on the checkout page.

Skip Shipping Step
------------------

 If you only have one shipping method, you can opt to hide the shipping step entirely by checking **Skip shipping step**.

Hide Coupon Code
----------------

 When **Enable to hide coupon code until link is clicked** is checked the coupon code will not appear until the user clicks a link labeled 'Have a promo code? Click here.'

Login Style
-----------

 By default, we show and hide the login form automatically based on whether we detect that the email address entered matches an existing account. To enable this behavior, select **Enhanced**.

 If you choose **WooCommerce Default**, this behavior will be replaced with an alert style message prompting the user to login above the form, the same as the native WooCommerce checkout page.

Registration Style
------------------

 When Enhanced is selected, we will override WooCommerce's registration settings to automatically generate a username and password for customers. They will just see a 'Create account' checkbox.

 When **WooCommerce Default** is selected, CheckoutWC will respect the WooCommerce settings and offer a password field like the native WooCommerce checkout page.

User Matching
-------------

 User Matching provides two features in one:

- When a customer with an account places a guest order using the same email address as their account, we attach the order to their account.
- When a customer who has placed guest orders registers for the first time with the same email address, we match previous guest orders to their new account.

 This feature is available to **Plus**, **Pro**, and **Agency** license holders.

Order Review Step
-----------------

For more information on Order Review Step, [see our guide here.](https://kb.checkoutwc.com/article/119-how-to-add-order-review-step)

[](https://kb.checkoutwc.com/article/119-how-to-add-order-review-step)Address Autocomplete
------------------------------------------------------------------------------------------

For more information on Address Autocomplete, [see our guide here.](https://kb.checkoutwc.com/article/72-how-to-enable-address-autocomplete)

SmartyStreets Address Validation
--------------------------------

For more information on SmartyStreets Address Validation, [see our guide here.](https://kb.checkoutwc.com/article/127-smartystreets-address-validation)

Mobile Options
--------------

Options that only affect the mobile view.

### Mobile Coupon Field

When **Show coupon field above payment options on mobile** is checked, a separate coupon field is shown on mobile devices separate from the one in Cart Summary. This is to make it easier for customers to find the coupon field on mobile.

### Show Credit Card Logos

By default we hide the credit card logos on mobile due to spacing issues. Check **Show credit card logos on mobile** to override this behavior.

### Cart Summary Mobile Label

Determines what the label for the cart summary is on mobile. By default it's 'Show order summary'