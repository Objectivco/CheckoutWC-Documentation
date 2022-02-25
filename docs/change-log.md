---
title: Change Log
slug: change-log
cats: Developers
---

<div>**Version 6.2.4 - 2022.02.11**

- Fix - Fix JS error when country field is not present.
- Fix - Fix issue with payment gateway change handlers that was causing an infinite AJAX refresh
- Fix - Fix fatal error caused by calling non-static method statically.
- Fix - Fix potential fatal error with Klarna Payments.
- Fix - Order failed text is now on the thank you page where it always should have been for those odd situations where a gateway sends someone to the order-received endpoint with a failed order.
- Fix - Fix improper detection of whether the selected payment gateway changed.
- Fix - Post code field no longer fires AJAX refresh on keydown to prevent poor UX with improper post code detection
- Improved - Refactored Google Address Autocomplete functionality to better handle different completion strategies for different countries.
- Development - Added unit testing for Google Address Autocomplete.

 **Version 6.2.3 - 2022.01.14**

 We have a lot of stuff in the works, but today we're releasing a tasty patch release that fixes some bugs and generally makes CheckoutWC better for everyone.

- New - Add support for YITH Points and Rewards 3.x
- Improved - Automatically exclude our JS files from WP Rocket transformations that break things.
- Improved - Added action before upsells are added to the cart: cfw\_before\_order\_bump\_add\_to\_cart
- Improved - When rendering a remove item link, we now pass it through the WooCommerce filter so that it picks up changes from other code.
- Improved - Refactored Google Address Autocomplete service. It's cleaner! It's faster! (maybe) And it's much easier to handle country by country edge cases.
- Fix - Fix multiple bugs with Checkout Field Editor (official WooCommerce extension)
- Fix - Clean up jQuery migrate warnings.
- Fix - Fixes for PayPal for WooCommerce Complete Payments gateway.
- Fix - Fix bug where error messages were not properly displayed if the error was not output in the form tag.
- Fix - Fix bugs with Thrive theme.
- Fix - Aborted AJAX calls are no longer logged as errors.
- Fix - Eliminated deprecated function call.
- Fix - Fix bug with Metro theme.
- Fix - Fixed bug where upsells were not discounted properly after being added to the cart.
- Fix - Fix bug where the city field was not validated if it was rendered off screen.
 
 **Version 6.2.2 - 2021.12.18**

 **'Tis the season to be conservative about plugin updates!** 🎄 If your store is humming along through the holiday rush, *you may want to wait a few weeks on this update.* But if you like the gifts below, receive them with our blessing. (After careful testing!)

- Fix - Fix potential fatal error with EU VAT Assistant compatibility module.
- Fix - Reworked order review step to hopefully allow it to work with more gateways.
- Fix - Fix JS error when address autocomplete is enabled but there are no address fields.
- Fix - Debounce scrolling to alerts.
- Improved - Refactored AJAX actions to use super.error() method and cleaned up unused properties/getters/setters.
 
 **Version 6.2.0/6.2.1 - 2021.12.13**

 **'Tis the season to be conservative about plugin updates!** 🎄 If your store is humming along through the holiday rush, *you may want to wait a few weeks on this update.* But if you like the gifts below, receive them with our blessing. (After careful testing!)

- Improved - Refactored Order Bumps to distinguish between different types of bumps and separate their logic.
- Improved - For products visible in the catalog, clicking an order bump's thumbnail will open the product page in a new window.
- Improved - Added a new function for grabbing all order bumps: cfw\_get\_all\_order\_bumps
- Improved - Added some unit tests to FormAugmenter
- Improved - Added unit testing to stat collection classes
- Improved - Added unit test to YITH Composite Products compatibility module
- Improved - If update\_checkout AJAX call fails, display a message letting customers know but return UI to normal state.
- Improved - If update\_checkout AJAX call fails, still trigger payment gateway init and updated\_checkout JS event like WooCommerce core does.
- Improved - If an error notice is already on the page and the same notice is on the next request, briefly animate the error notice with a shaking effect so that customers realize the error still applies.
- Fix - Fix a loophole that allowed people to get order bump special pricing without qualifying for the bump.
- Fix - SmartyStreets now works when shipping address is forced to billing address.
- Fix - Implemented automatic LTR &gt; RTL CSS conversion.
- Fix - Adjust priority of our assets to avoid a conflict with Divi.
- Fix - Significant fixes for WP Rocket's handling of WooCommerce fragments and how this affects Side Cart.
- Fix - Similarly, we made sure side cart works with the popular plugin Disable Cart Fragments.
- Fix - If an order bump's offer product is on sale, that price is used as the base price for any bump specific discounting.
- Fix - Fix bug with Free Gifts for WooCommerce that caused the Side Cart not to open when quantity triggered free gift.
- Fix - Fixes for Order Delivery Date plugin.
- Fix - Fix for EU VAT Assistant and digital only orders.
- Fix - Fix bug that prevented order stats from being collected for many sites.
- Fix - Fix bug with WooFunnels Order Bump Upsells that caused AJAX update loop
- Fix - When upgrading CheckoutWC, clear WP Rocket's fragment cache
- Fix - Fix bugs in how cart item data was displayed, particularly with WooCommerce Product Add-ons
- Fix - Fix bug where quantity of side cart button did not update when cart updated.
- Fix - Fix potential error if first gateway in session is null
- Fix - Fix bug with WooCommerce Memberships that caused AJAX calls to fail when restriction mode was set to redirect.
 
 **Version 6.1.7 - 2021.11.19**

- New - Added support for Free Gifts for WooCommerce
- Improved - Added missing woocommerce\_before\_thankyou hook
- Improved - Exclude our JS and CSS from WP Rocket optimizations automatically
- Improved - Refactored cfw\_form\_attributes() and added a new filter for adding your own attributes: cfw\_form\_attributes
- Fix - Fix bug where invalid post codes did not generate an error message
- Fix - Fix bug where null cart item data was still displayed on checkout page.
- Fix - Fix bugs with UK addresses and SmartyStreets
 
 **Version 6.1.6 - 2021.11.10**

- New - Added preliminary support for WooCommerce EU VAT Assistant.
- Fix - Fix bug with method that determines if all shipping packages have a selected shipping method
- Fix - Regenerated stale MO files for de\_DE and de\_DE\_formal translations. *Der Fehler tut uns leid!*
- Fix - Fix missing filter that caused WooCommerce Product Bundles component items to be listed on the thank you page in conflict with the product page settings.
- Misc - Update WooCommerce tested version to 5.9.0
 
 **Version 6.1.5 - 2021.11.8**

- Improved - Added filter to control whether side cart items link to the product page. Filter: cfw\_side\_cart\_link\_item
- Fix - Fix bug where solid side cart icons fill color was set to none.
- Fix - Make sure elements with cfw-side-cart-open-trigger class have pointer cursor.
 
 **Version 6.1.4 - 2021.11.5**

- New - New side cart setting to hide floating side cart button when cart is empty.
- New - Order Bumps admin view now displays revenue that bump has captured. (Past revenue is estimated)
- Improved - When trust badge doesn't have a title or description, image is now displayed full width
- Improved - Added description to make it clear you can add embedded scripts to trust badge description for dynamic badges such as Norton Security.
- Improved - Added beta support for using Astra's header and footer on the checkout page. Requires loading theme styles which could cause conflicts.
- Improved - Set fill to none on side cart icon to prevent theme conflicts.
- Fix - Fix edge case where radio buttons had improper label styles.
- Fix - Fix bug where HTML tags ended up in field placeholders.
- If a label has an HTML tag present in it, display it as a conventional, non-floating label.
- Fix - Fix issue with UpSolution Core plugin by preventing it from loading styles on the checkout page.
 
 **Version 6.1.3 - 2021.11.2**

- Hotfix - Fix bug that caused side cart links to open in a new tab/window.
 
 **Version 6.1.2 - 2021.11.2**

- Improved - Side Cart item titles and images now link to the product page.
- Improved - When enabling cart item links in CheckoutWC &gt; Cart Summary, both title and image now link to the product page.
- Fix - Fix issue with WooCommerce Advanced Shipping that caused shipping to be rendered as 'Free!' inappropriately
- Fix - Fix JS error when no payment methods are available.
- Fix - When applying a coupon, any notices that appear will be cleared on the next AJAX refresh.
- Fix - Fix an issue with Avada that caused inline styles to be rendered to the page when they shouldn't be.
- Fix - Fix some German translations in de\_DE and de\_DE\_formal
- Fix - Fix issue with Side Cart where inclusive taxes (VAT) was not handled properly when calculating the free shipping amount remaining.
- Fix - Fix issue where stat collector only sent 6 days of stats instead of 7.
- Fix - Fix issue where stat collector sent staging site stats.
 
 **Version 6.1.1 - 2021.10.27**

- Fix - Fix styling issue with secondary buttons such as the apply coupon button.
 
 **Version 6.1.0 - 2021.10.27**

- New - Added icon picker to Side Cart options!
- New - Added settings for side cart icon width and color.
- New - Added option to enable coupons on side cart.
- New - Added shortcode for placing a side cart launcher anywhere on your site. \[checkoutwc\_cart\]
- Improved - Improved how order bumps are shown in side cart so they don't cover the cart items on small mobile devices.
- New - Added action to allow adding content when side cart is empty: checkoutwc\_empty\_side\_cart\_content
- Fix - Fix when no shipping method is selected, don't show 'Free!'
- Fix - Fix issue with Avada 7.5
- Fix - Fix issue where AJAX refresh happens twice on initial page load.
- Fix - Fix an issue with mobile
- Fix - Fix issue with SplitIt gateway
- Fix - Fix JS error with state not being a part of locale object.
- Fix - Fix left over var\_dump in UpdatesManager.
- Fix - Fix subtle styling bug with accordions that has been lurking forever.
 
 **Version 6.0.7 - 2021.10.22**

- Improved - Added filters to WooCommerce Gift Cards output to allow heading, label, and placeholder to be changed.
- Fix - Disable JS that smoothly resized country, postcode, and state fields when switching countries because it's causing major the mobile view to zoom in and zoom out during refreshes on some sites.
- Fix - Account exists check was firing even when email field was empty.
- Fix - Fix issue where turning off checkout cart editing feature turned off the ability to change quantities or remove items on the side cart.
 
 **Version 6.0.6 - 2021.10.21**

- New - Added Romanian translations
- Improved - Order bumps now appear in the side cart when you enable the option in WP Admin &gt; CheckoutWC &gt; Side Cart
- Improved - Improved side cart styling
- Improved - Refactored Google Address Autocomplete JS
- Improved - Refactored Fetchify Address Autocomplete JS and
- Fix - Fix bug where Plus plan holders could see Side Cart settings in admin. Settings are now hidden unless you are a Pro or Agency license holder.
- Fix - Fixed styling issues with Fetchify Address Autocomplete and Glass theme / admin bar
- Fix - de\_DE\_formal is now a separate locale from de\_DE. Thanks, Jörg!
- Fix - Free Shipping progress bar now shows decimal values when necessary.
- Fix - Fix more CSS conflicts with Side Cart and random themes and plugins
 
 **Version 6.0.5 - 2021.10.16**

- Improved - Implement woocommerce\_cart\_item\_class so that plugins that need it can use it.
- Fix - Harden up styles to help mitigate Side Cart styling conflicts with themes.
- Fix - Fix issue where Resurs gateway needs classes on parent element to be in a specific order. (Yes, you read that right)
- Fix - Fix bug with merging locale data that resulted in JS errors for some stores.
- Fix - Prevent Astra Addon from loading styles on the checkout page.
- Fix - Fix date picker z-index with Local Pickup Plus.
- Fix - Fix bug with how we ran our AJAX updates on the checkout page that resulted in update\_shipping\_method not being set on requests. This caused major issues with Local Pickup Plus.
- Fix - Fix Fetchify styling.
- Fix - Fix responsive styles between mobile and desktop sizes where styling was broken.
- Fix - Implemented jQuery.scroll\_to\_notices from WooCommerce core for compatibility. *This should also fixes JS errors with WooCommerce PayPal Payments.*
- Fix - Make primary action button on mobile 100% width and place it before the secondary action (such as 'Return to shipping method')
- Fix - Fix issue where place order button was not 100% width on mobile.
- Fix - Fix styling of breadcrumbs on Futurist template.
 
 **Version 6.0.4 - 2021.10.13**

- Hotfix - Remove PHP 7.4 only code that causes fatal errors on older servers.
 
 **Version 6.0.3 - 2021.10.12**

- Improved - Forcefully re-enable cart fragment system when side cart is active.
- Fix - Fix bug where WooCommerce would redirect somewhere else instead of opening Side Cart. (When Side Cart is enabled our 'Skip cart step' feature is ignored)
- Fix - Fix bug where side cart didn't open on adding an item to cart if AJAX add to cart was turned off.
- Fix - Tweak styling of side cart to give header some more room to breathe.
- Fix - Native WooCommerce 'View cart' buttons should now open side cart.
- Fix - Added aria-label to floating cart button for screen readers.
- Fix - Fix potential fatal errors.
- Fix - Fix bug with SmartyStreets where it would break if your lookups were depleted.
- Fix - Fix bug with SmartyStreets where multiple requests were made for each lookup.
- Fix - Fix bug with SmartyStreets where modal would not close when clicking button to accept address.
- Fix - Fix esoteric bug with Resurs Bank gateway.
- Fix - Fix admin label for Side Cart 'Free Shipping Message'
- Fix - Use native WooCommerce unknown error message when gateway returns failure with no error messages.
 
 **Version 6.0.2 - 2021.10.11**

- Fix - Fix translation of continue shopping button
- Fix - Fix fatal error when cart or order item thumbnail is null
- Fix - Fix box-sizing issue that was causing things to render a few pixels offset
- Fix - Stop Flatsome from uppercasing cart item titles in side cart
- Fix - Stop Storefront theme from adding animation spinner to side cart update blockUI styling
- Fix - Fix issue with Futurist template breadcrumbs wrapping
- Fix - Fix issue where Futurist breadcrumb accents where missing
 
 **Version 6.0.1 - 2021.10.08**

- Improved - Add a separate setting for the background color of the free shipping progress bar.
- Fix - Fix issues with Side Cart and glass theme.
 
 **Version 6.0.0 - 2021.10.08**

- NEW! Side Cart is here and it's beautiful and lightning fast. Adding items to the cart opens a flyout cart from the right side of the screen that perfectly matches the cart experience on the checkout page and includes extras like a free shipping progress bar. This feature is available to all Pro plan and above subscribers.[ You can see a demo here.](https://demo2.checkoutwc.com)
- NEW! International Phone Field allows merchants to validate that the phone number entered is a valid phone number in the country selected. And it allows you to choose how the phone is stored when the order is submitted - this can help greatly with fulfillment services that require a specific format and valid phone numbers to work correctly.
- Improved - Upgraded Bootstrap grid from 4.x to 5.x
- Improved - Various performance improvements.
- Fix - Fixed issue on checkout page where quantity bubble on cart items was cut off.
- Fix - Lots of other little fixes we found. You know, the real 6.0 release is the commits we made along the way.
 
 **Version 5.3.11 - 2021.10.04**

- Hotfix - Ok, we didn't get that quite right:  
     Fix cfw\_get\_shipping\_total()
    
     Essentially invert logic of cfw\_get\_shipping\_total() so that it follows the logic of WooCommerce's cart/cart-shipping.php template by first checking the available methods, and then descending into other checks.
    
     This also requires changing how cfw\_show\_shipping\_total() determines whether to show the shipping total. Since error states are part of the shipping total, those are pushed further down to cfw\_get\_shipping\_total() and instead we only check that we have shipping enabled and that the cart has items.
 
 **Version 5.3.10 - 2021.10.04**

- Fix - Fix bug that caused 'Enter your address to view shipping options' to be displayed when the phone field was empty
- Improved - Refactor how we handle activation / deactivation routines
 
 **Version 5.3.9 - 2021.09.27**

- Improved - Add skip cart feature in CheckoutWC &gt; Checkout
- Fix - Fix bug that caused 'Free!' to show up on some orders where a shipping address had not been entered.
- Fix - Fix bug with SmartyStreets that caused the continue to payment button to be shown when it shouldn't be.
- Fix - Fix bug with Order Bumps when Offer Product is deleted.
 
 **Version 5.3.8 - 2021.09.16**

- Hotfix - Fix issue with styling of payment methods / billing address accordions on Glass theme
 
 **Version 5.3.7 - 2021.09.15**

- New - Bumped minimum PHP version to 7.1 since one of our existing dependencies already required PHP 7.1, setting an implicit minimum version.
- Fix - Fix bug with WooCommerce payments where the radio button for selecting credit card disappeared.
- Fix - Fix bug where shipping methods were blocked and wouldn't unblock
- Fix - Fix for Avada thank you page and view order page
- Fix - Fix for Avada styling of HTML element
- Fix - Fix for WooCommerce Gift Cards and coupon code AJAX. Now uses native WooCommerce AJAX for applying coupons.
- Fix - Fix a poorly translated French phrase.
- Fix - Fix up WooCommerce Shipment Tracking output and remove duplication
- Fix - Move theme styles / scripts suppression code outside of CompatbilityAbstract so it only runs once.
- Fix - Fix issue with whitespace on the right side of page on iPhones when using WooCommerce PayPal Payments
- Fix - Don't show optional in placeholder for fields that Brazillian Market changes
- Improved - Added filter for distraction free portal template redirect priority: cfw\_template\_redirect\_priority
- Improved - Added filter for disabling existing account lookup by email: cfw\_enable\_account\_exists\_check
- Improved - Run initial AJAX update on page load faster (same speed as WooCommerce native checkout page)
- Improved - Added filter for determining when an order bump displays: cfw\_display\_bump
 
 **Version 5.3.6 - 2021.09.03**

- Improved - Tightened up timing of first AJAX refresh on checkout page to match core WooCommerce.
- Improved - Added support for Post NL 4.x
- Improved - If no valid shipping methods are available we now hide the 'Continue to payment' button to avoid confusion
- Fix - Fix issue with thank you page and Avada theme
- Fix - Protect against null cart items causing fatal error
- Fix - Fix order bumps fetch to include more than 5 items.
- Fix - Fix Klaviyo bug that caused the SMS notice to be separated from the checkbox.
- Fix - Fix Klaviyo bug where SMS checkbox had same name as newsletter checkbox.
- Fix - Fix potential styling issues with WooCommerce PayPal Payments when "Pay in X" notice is present
- Fix - Fix duplicated checkboxes with latest Klaviyo plugin update. **(Please update Klaviyo after installing this release)**
- Tweak - Slightly changed output position of Klaviyo checkboxes.
- Tweak - Added $mobile boolean variable to cfw\_before\_coupon\_module action
 
 **Version 5.3.5 - 2021.08.20**

- Improved - Support WooCommerce 5.6.0 built in support for Shipping Phone field.
- Improved - Add compatibility for WooCommerce Gift Cards coupon input add-on plugin
- Improved - Switch Amazon Pay logo to SVG for vector retina rendering goodness.
 
 **Version 5.3.4 - 2021.08.04**

- Fix - Fix express checkout button rendering for WooCommerce payments.
 
 **Version 5.3.3 - 2021.08.04**

- Improved - Beta Support for WooCommerce Payments express checkout buttons. This is largely untested due to the difficult of testing WooCommerce Payments in a dev environment. Please let us know if it works for you.
- Improved - Added additional CSS custom properties that make it possible to control loading "shimmer" animation during refreshes
- Fix - Fix location of mobile coupon output. Now appears above the payment methods as described by the option in CheckoutWC &gt; Checkout
- Fix - Fix a potential fatal error
- Fix - Order Bumps filter no longer appears on the orders list when there are no order bumps
- Fix - Shore up order submission JS to match WooCommerce core more closely
- Fix - Make sure wc\_checkout\_params.checkout\_url is the right AJAX submission endpoint on our checkout page
- Fix - Fix issue with YITH points and Rewards notice not appearing
 
 **Version 5.3.2 - 2021.07.21**

- New - Futurist theme now has full access to breadcrumb color settings
- Improved - Added cfw\_klaviyo\_output\_hook filter to determine where Klaviyo outputs its stuff
- Improved - Added cfw\_shipping\_free\_text filter to set the text when shipping is free
- Fix - Fix issue with location of cfw\_before\_payment\_method\_heading action and fragment updates
- Fix - Update German translation of promo code
- Fix - Fix issue with mismatched label and placeholder for fields like post code based on country locale strings from WooCommerce core
 
 **Version 5.3.1 - 2021.07.10**

- Fix - Fix issue where company field didn't trigger a refresh.
- Fix - Fix cart summary mobile background color with new settings scheme. Added a new Cart Summary Mobile Background Color setting
- Fix - Fix issue where current order status was not reflected when viewing an order if the current status was not set as one of the status progressions in the Thank You Page settings.
 
 **Version 5.3.0 - 2021.07.6**

 This is a pretty big release! **As always, we recommend testing on a staging site before updating your live site!**

- New - Added new address autocomplete service - [Fetchify](https://kb.checkoutwc.com/article/136-fetchify-address-autocomplete)!
- New - Filter WooCommerce Admin orders screen by whether the order contains Order Bumps.
- New - New color settings for breadcrumbs and accent colors.
- New - Refactored color settings to use Custom CSS Properties.
- New - It's now possible to remove cart items that don't have an adjustable quantity.
- New - Added option to CheckoutWC &gt; General to hide the CheckoutWC admin menu bar button on non-CheckoutWC pages.
- Improved - Added cfw\_is\_thank\_you\_page\_active() function to let developers determine if the thank you page is turned on.
- Improved - Fields with attribute data-persist=false won't be locally cached with Garlic.
- Improved - JS build target moved from es5 to es2015.
- Improved - Changing company field now refreshes checkout since it is visible in the order review panes.
- Fix - Fix issue with account exists checks running even when login form was set to use WooCommerce login.
- Fix - Fix issue with WooCommerce PayPal Payments fields rendering with the wrong size.
- Fix - Fix visual glitch with rounded borders on accordions (shipping methods, payment methods, billing address) that caused the border to have a small white break at the corners
- Fix - Fix issues with SmartyStreets and address\_2
- Fix - Fix issue with Klaviyo checkbox being output twice.
- Fix - Fix issue with order bump not showing if offer product stock wasn't managed.
- Fix - Fix issue with Php Snippets and the backslash character.
- Fix - Fix PHP warning with WooCommerce Square gateway
- Fix - Fix refactored how we handle shipping totals to more accurately display conditions such as no shipping methods being available, especially when using more than one shipping package.
- Fix - If value exists on page load, don't override it with Garlic.
- Fix - Removed cfw-field-persistence-loaded JS event since it didn't work.
- Fix - Fix issue with CartFlows React UI.
- Fix - Fix issue where billing\_email didn't match logged in user's email.
- Fix - Fix mobile styling issue with WooCommerce notices that contain buttons.
- Fix - Fix issue with Parsley field validation message translation and Weglot.
 
 **Version 5.2.4 - 2021.07.02**

- Hotfix - Fix issue with Avada 7.3.1
 
 **Version 5.2.3 - 2021.06.15**

- Fix - Fix issue with WooCommerce Germanized checkboxes next to the place order button
 
 **Version 5.2.2 - 2021.06.14**

- Hotfix - Fixes for Avada 7.4. [PLEASE READ THIS DOC BEFORE CONTACTING SUPPORT.](https://kb.checkoutwc.com/article/65-avada-template-layout-problems)
 
 **Version 5.2.1 - 2021.06.14**

- Hotfix - Fix output of WooCommerce Germanized checkboxes
 
 **Version 5.2.0 - 2021.06.10**

- New - Order Bumps can now be configured to show if one or more category of products is in the cart!
- New - Support for ConverKit for WooCommerce
- Improved - If an Order Bump becomes invalid because the cart changed, we "undiscount" the bump until the cart satisfies the bump conditions.
- Improved - Added JavaScript validation to Order Bumps editor.
- Improved - When showing discounts on cart items, render Order Bumps price correctly.
- Fix - Fix issue with WooCommerce PayPal Payments that caused the PayPal buttons not to appear.
- Fix - You can no longer select a variable product parent as an offer product.
- Fix - Bumps cannot satisfy the display conditions for other bumps.
- Fix - Fix compatibility with woocommerce\_checkout\_redirect\_empty\_cart and woocommerce\_checkout\_update\_order\_review\_expired hooks.
- Fix - Added a workaround for Authorize.net and order review step
 
 **Version 5.1.2 - 2021.06.09**

- Hotfix - Fix issue with Chrome autofilling fields bug and one page checkout setting.
 
 **Version 5.1.1 - 2021.06.08**

- Fix - Fixes for Klaviyo SMS checkbox and disclaimer location
- Fix - Fix issue with Trusted Payments gateway
- Fix - Fix issue where express checkout container showed up when no express buttons were present
- Fix - Fix bug with Chrome autofilling fields on previous steps
- Fix - Fix admin conflict with Formidable Forms and MapSVG
 
 **Version 5.1.0 - 2021.06.04**

- New! Order Bumps can now be used as Upsells. Check out our documentation here: <https://kb.checkoutwc.com/article/126-order-bumps>
- New - Support for WooCommerce Pakettikauppa
- New - Support for Woo Finvoicer
- Fix - Fix issues with TM Extra Product Options and Order Bump discounts
- Fix - Add login prompt to PayPal for WooCommerce review order screen
- Fix - Fix issue with WooCommerce Checkout Fields Editor Pro from Acoweb where fields were readonly
- Fix - Add beta support for ThemeHigh's popular Checkout Field Editor.
- Fix - Fix issues with WooCommerce Juno
- Fix - Fix issues with Brazilian Market on WooCommerce
- Fix - Fix JavaScript error in express checkout button check
- Fix - Fix validation of extra shipping fields where fields don't have labels
- Fix - Fix styling of select2/selectWoo select fields
 
 **Version 5.0.5 - 2021.05.27**

- Fix - Fix issue with Parsley validation of checkboxes
- Fix - Fix translation for WooCommerce Gift Cards
- Fix - Fix issue where Elementor header / footer didn't show up on thank you page
- Fix - WP admin bar now shows up on thank you page if you're logged in
- Fix - Fix issue with Spanish addresses autocompleting state incorrectly
- Fix - Fix issue with fields laying out incorrectly when country switched
- Fix - Fix button styling on address verification modal (SmartyStreets)
- Fix - Billing address is always shown when Brazilian Market on WooCommerce is active.
- Fix - Fix glitches with payment request buttons container showing up when no buttons were available.
 
 **Version 5.0.4 - 2021.05.20**

- Fix - Fix problem with PayPal for WooCommerce that caused billing address fields to not sync over correctly from logged in session.
- Fix - Fix PHP warning
- Fix - Fix issue where Trust Badge didn't appear to save unless you added an image
- Fix - Fix how trust badges lay out on frontend without images
- Fix - Adjusted priorities of address fields to match core more closely
 
 **Version 5.0.3 - 2021.05.19**

- Fix - Fix bug with one page checkout not firing order submit handlers properly.
- Fix - Fix styling bugs with content loader.
- Fix - Fix JS errors with Amazon Pay.
- Fix - Fix bug with create account checkbox not auto checking.
- Fix - Fix PHP 8 deprecation notice.
 
 **Version 5.0.2 - 2021.05.18**

- Hotfix: Fix issue where billing address fields weren't synced from shipping address fields.
- Fix: Fix glitches with admin bar
- Fix: Fix issue with view order URL being styled incorrectly
- Fix: Fix issue with styling of checkboxes
- Fix: Fix issue with Canada city being filled improperly with Google Address Autocomplete.
- Fix: Fix issue where Amazon button could render incorrectly for a few seconds.
- Improved: Added mechanism for custom validation of custom fields with parsley.js
 
 **Version 5.0.1 - 2021.05.18**

- Hotfix: Fix bug where translations did not load
- Hotfix: Fix bug where Trust Badges settings did not appear to save
 
 **Version 5.0.0 - 2021.05.17**

 Major new version! This release comprises over 700 commits - we didn't hold back. We're excited for you to try it, but you should do proper testing before updating. **Before updating your live site, PLEASE TEST ON STAGING.**

- New - Order Bumps (Pro or higher plan)
- New - SmartyStreets Address Validation (Pro or higher plan)
- New - Trust Badges
- New - Footer menu location for adding footer links to the checkout page.
- New - Redesigned admin pages
- New - Estonian translations
- Improved - Support for latest Square gateway express buttons (Apple Pay, Google Pay, etc)
- Improved - Refactored code base for faster more robust performance
- Fix - Fix issue with Alabama being selected by default when it shouldn't be
 
 **Version 4.3.8 - 2021.05.11**

- Hotfix: Fix Amazon Pay. Should work with Amazon Pay 1.0 and Amazon Pay 2.0, including both the legacy integration method and the new API. However, the new API is **NOT fully tested** due to the urgent nature of releasing this fix. **We do NOT recommend you reconnect to the Amazon API until you have *FULLY* tested on a staging site.**
- Fix - Fix glitch with non-shipped orders and PayPal for WooCommerce review screen.
- Fix - Fix some styling issues with CommerceKit
- Improved - Added cfw\_thank\_you\_page\_map\_address filter to allow overriding the map address on the thank you page.
- Improved - Added symlink for de\_DE\_formal locale to de\_DE.
 
 **Version 4.3.7 - 2021.05.06**

- Fix - Fix how we set language for Google Address Autocomplete
- Fix - Fix fatal error with old version of Klaviyo by adding version check
 
 **Version 4.3.6 - 2021.05.04**

- Improved - Set language for Google Places library so that autocomplete suggestions are in the correct locale
- Fix - Fix Klaviyo newsletter checkbox position
- Fix - Fix issue with WooCommerce Conditional Shipping and Payments notices not being displayed on update\_checkout
 
 **Version 4.3.5 - 2021.04.26**

- Hotfix - Fix invalid reference to settings manager in WooCommerce Germanized compatibility class.
 
 **Version 4.3.4 - 2021.04.26**

- New - Compatibility with Neve theme
- New - Vietnamese translations
- Fix - Fix bugs with validation of billing address when order review step is enabled
- Fix - Fix styling issues with order review step total
- Fix - Parse house number if Google Maps doesn't have address in their DB
- Fix - Workaround for Dutch addresses and Address Autocomplete to properly map city field
- Fix - Fix for WooCommerce Germanized terms and conditions and order review step
 
 **Version 4.3.3 - 2021.04.01**

- Fix - Fix PHP 8 warnings / notices.
- Fix - Fix for Uncode theme
- Fix - Fixes for Avada 7.3
- Fix - Fix for Stripe (official) gateway that prevented Apple Pay / Google Pay when phone fields were required.
 
 **Version 4.3.2 - 2021.03.30**

- Fix - Fix bug with WooCommerce Germanized where cart items were not visible
- Fix - Fix issue with Stripe for WooCommerce and iDEAL that made the bank dropdown not selectable.
- Fix - Fix PHP 8 warnings.
 
 **Version 4.3.1 - 2021.03.29**

- Hotfix - Fix issue where gateway icons could be way too tall.
- Hotfix - Fix issue where AJAX requests response was being cached occasionally in Safari.
 
 **Version 4.3.0 - 2021.03.26**

- 🎨 New: During refreshes checkout sections now have a sweet new 'loading shimmer' effect rather than fading out.
- Improved: Page now refreshes faster on first load
- Improved: Added missing aria description to field output.
- Fix - Fix edge cases where fatal error could be fired if a shipping method isn't a proper shipping method.
- Fix - Fix bug that caused fractional quantities like 0.5 to remove an item from the cart.
- Fix - Fix issue where billing address fields were synced from shipping address at the wrong time on page load. Now happens after field values have been restored from cache.
- Fix - Fix styling of cart total on mobile
- Fix - Fix issue where JS error was thrown when Checkout Add-ons for WooCommerce was activated.
- Fix - Fix bug where post code was not set to optional or required properly when switching countries.
- Fix - Fix bugs with Stripe and Order Review Step feature.
- Fix - Fix issue with New Zealand addresses and Google Address Autocomplete.
- Fix - Fix improper implementations of debounced that were not debouncing.
- Fix - Fix issue where cart items were being modified during refresh when there were no changes.
- Fix - Fix bug with custom attributes on fields that caused them to be output improperly.
- Fix - Fix bug with Free Gifts for WooCommerce that caused items not to show up when cart was modified to satisfy gift conditions.
 
 **Version 4.2.0 - 2021.03.18**

- Improved - Cart updates now happen in normal update\_checkout refresh - saves an extra AJAX call.
- Improved - Performance: On page load, multiple AJAX refreshes would run. Now only one will run.
- Improved - All compatibility classes are now singletons with accessible instances
- Improved - Refactored compatibility module system to improve
- Improved - Some light refactoring of our JS to decouple the code and prepare for larger refactors later.
- Fix - Fix styling issue with coupons on Futurist theme.
- Fix - Fix bug where removing YITH composite product didn't remove components.
- Fix - Fix for Avada and the thank you page.
- Fix - Fix CSS conflict with Flatsome theme.
- Fix - Fix styling bugs with Klarna Checkout.
- Fix - Fix bugs with Brazilian Market
- Fix - Fix bug where Smart Coupons 'bounced' multiple times on page load
- Fix - Fix change how we resolve state with Google Address Autocomplete to handle more countries correctly
 
 **Version 4.1.1 - 2021.03.05**

</div>- New - Bulgarian translations
- Fix - Fix potential error in Avada compatibility module
- Fix - Fix bug with Address Autocomplete that resulted in house\_number showing up in address field 1
- Fix - Fixes for Brazilian Market (Extra Checkout Fields for Brazil)
- Fix - Fixes for country / state field changes that resulted in inconsistent states or wrong labels.
- Fix - Fix JS error on order pay page that could prevent the page from functioning.

 **Version 4.1.0 - 2021.02.26**

- New - Added support for Sumo Subscriptions
- New - Added Czech translations
- Improved - Added custom event (cfw-fire-udpate-cart-action) for triggering update\_cart event
- Improved - Added woocommerce\_view\_order hook (but surpassed default actions on hook that are redundant)
- Fix - Fix styling issue with Pro theme
- Fix - Fix issue with billing address sync from shipping fields to correct issues with gateways and ensure the session address data is properly stored / retrieved
- Fix - Fix issue with SEPA gateway and Stripe For WooCommerce (Payment Plugins)
- Fix - Fix for issue where other plugins look for a particular class when checking notices on page
- Fix - Fix issue with SplitIt payment gateway
- Fix - Prevent fatal errors when gateway isn't a proper gateway instance or no gateways are enabled

 **Version 4.0.7 - 2021.02.22**

- Hotfix: Fix another Amazon Pay issue that caused the shipping state to be hidden.
- Fix: Fix issue with Google Address autocomplete and premise / subpremises.

 **Version 4.0.6 - 2021.02.19**

- Hotfix: Fix issue with latest Amazon Pay gateway update that caused the shipping address fields to be hidden.

 **Version 4.0.5 - 2021.02.11**

- Fix - Fix issues with SendCloud update.
- Fix - Fix issue with Flatsome and WooCommerce Germanized.
- Fix - Fix potential fatal error on thank you page.
- Fix - Fix styling for Google Pay button with Stripe for WooCommerce (PaymentPlugins) gateway.

 **Version 4.0.4 - 2021.02.04**

- New - Support for saved Addresses for WooCommerce.
- Fix - Fix bug with Woocommerce Side Cart Premium that caused endless refreshes when paired with Google Address Autocomplete feature.
- Fix - Fix inefficiency with Address Autocomplete feature that caused redundant events to be queued when using autocomplete more than once.
- Fix - Fix bug with TranslatePress that caused AJAX output to contain get text wrapping strings.
- Fix - Removed old Braintree for WooCommerce (PaymentPlugins) JS compatibility code that is no longer needed.

 **Version 4.0.3 - 2021.02.01**

- New - Added Korean (ko\_KR) translations
- Fix - Fix issue where company wasn't sent with update\_checkout
- Fix - Fix issue where shipping address review had stale data.
- Fix - Fix JS error when no payment methods are available.
- Fix - Fix issue where place order button HTML was not updated during refreshes.
- Fix - Fix issue with missing compatibility module JS
- Fix - Fix styling of Stripe for WooCommerce payment request buttons.
- Fix - Fix issue with payment gateway being reset to first selected gateway during refreshes.
- Fix - Fix issue where summary showed innert 'Change' links on PayPal for WooCommerce review page.

 **Version 4.0.2 - 2021.01.22**

- New - Added Croatian and Chinese Traditional (Taiwan) translations
- Enhanced - Removed vestigial cfw\_updated\_checkout event as some gateways had implemented it to correct issues that are no longer issues. This prevents potential problems from events running twice.
- Enhanced - Implemented woocommerce\_quantity\_input\_max filter to make sure our quantity stepper obeys the rules on maximum quantity.
- Fix - Fix a few PHP notices.
- Fix - Fix issue where 'Change' link showed up by the shipping method in the review panels when 'Ship shipping step' was enabled.
- Fix - Fix issue where you could enter more than the allowed product quantity in the JS prompt that appears when you click 'Edit'.
- Fix - Fix issue where order review step totals didn't properly update.
- Fix - Fix issues when applying a coupon code that makes an order free.
- Fix - Fix issue where removing a 100% off (free) coupon resulted in the payment method label not being displayed in the review panels.

 **Version 4.0.1 - 2021.01.15**

- Hotfix: Fix bug with pre\_option\_ filter that caused WooCommerce style registration to fail.
- Update Norwegian translations.

 **Version 4.0.0 - 2021.01.14**

 This release took about 6 weeks to finish and over 117 commits. This release is more about refinements and thoughtful refactors than new features, but it does have some new features too!

 **Please test carefully on a staging site before updating.**There shouldn't be any breaking changes, but any release of this size is certain to have bugs that were missed during the development and testing processes.

- **New Premium Feature:**Order Review Step - Order Review Step adds a tab after the payment tab with a full summary of the order information and totals above the place order button. This should be especially helpful to German stores, and other stores located in jurisdictions that require full disclosure before order submission.
- **Enhanced Remove Coupon:**Removing coupons now happens with an AJAX refresh instead of reloading the page.
- **New:**Support for MyShipper
- **New:**Support for Iconic WooCommerce Delivery Slots
- **New:**Complete parity with WooCommerce core on checkout refreshes. We now fire updated\_checkout on every refresh instead of selectively. Should iron out various glitches we have had with 3rd party add-ons.
- **New:**Lithuanian translations.
- **New:**Support for Shoptimizer
- **Enhanced:**It's now possible to use a filter and set a step amount for quantity adjustments.
- **Enhanced:**You can now click on the entire row of payment methods and other accordions rather than clicking specifically on the text label.
- **Enhanced:**Added various new filters. Documentation coming soon!
- **Enhanced:**Added docblock documentation for all our actions and filters to make updating our documentation easier.
- **Enhanced:**Refactored our compatibility class loader.
- Fix: Fixes for Local Pickup Plus
- Fix: Fixes for WooCommerce German Market
- Fix: Fixes for OceanWP themes
- Fix: Fixes for latest version of Avada theme
- Fix: Updates to French translations
- Fix: More robust parsing of error messages during checkout submit.
- Fix: Fix bugs with WooCommerce Country Based Payments
- Fix: Fix issues with WooCommerce Order Delivery Date
- Fix: Fix stale selector issue with payment method state cache during updates.
- Fix: Fix for Culqi payment gateway and other gateways that use the order pay receipt hook.
- Fix: Fix for error messages that could not be properly hashed.
- Fix: Fix for MyParcel styling
- Fix: Fix review pane address references to pickup changes and not pull from stale session info.
- Fix: Fix JS errors on order pay page.

 **Version 3.13.3 - 2020.11.26**

- New: Support for WooCommerce Subscription Gifting.
- Fix: Fix 'No shipping options' string to match WooCommerce core. This enables proper translation.

 **Version 3.13.2 - 2020.11.23**

- Fix: Revert Amazon Pay changes from 3.13.0 that caused issues with missing email fields.
- Add cfw\_payment\_methods\_ul\_start and cfw\_payment\_methods\_ul\_end actions.

 **Version 3.13.1 - 2020.11.19**

- Hotfix: Fix tiny CSS styling issue with return to previous step links that caused them to break onto two lines.

 **Version 3.13.0 - 2020.11.19**

- New: CheckoutWC now works with [reCaptcha for WooCommerce](https://woocommerce.com/products/recaptcha-for-woocommerce/).
- New: Added support for WooCommerce Enhanced Coupon Features Pro.
- Improved: Refactored update\_checkout AJAX refresh code to align it with WooCommerce core. This fixed some edge case bugs and simplified the code.
- Improved: We no longer hide settings from WooCommerce &gt; Settings &gt; Accounts &amp; Privacy. We mark them with an asterisk and a note so you know which ones may be overridden by CheckoutWC.
- Improved: Added an internal logging service for logging JS errors and events.
- Improved: Added some button styling for buttons in alerts.
- Fix: Don't show WPWeb Social Login buttons for logged in users.
- Fix: Fix issues with Pimwick Gift Cards. We're no longer doing a full integration with this plugin as the code is too brittle and requires us to copy their templates and then maintain them. Consequently, the gift card field will no longer show up under the promo card field.
- Fix: Fix issues with WordPress theme loader (still experimental) and Square gateway
- Fix: Fix issues with Checkout Add-ons and Select2 fields.
- Fix: Fix bug where admin area of Checkout Field Editor didn't hide unusable areas.
- Fix: Fix issue with WooCommerce Product Add-ons cart item data.
- Fix: Fix styling of Braintree / Stripe for WooCommerce payment request buttons (PaymentPlugins gateways)
- Fix: Fixed an undefined index notice.
- Fix: Fix mobile styling of mobile cart summary header.
- Fix: Fix cfw-payment-tab-loaded event
- Fix: Fix issue where Stripe CC field was rendered with an invisible placeholder on mobile safari / iOS.
- Fix: Fix issue where Amazon Pay button could show up and be unclickable.
- Fix: Added a way to re-enable field validation when using Amazon Pay. Filter: cfw\_amazon\_suppress\_shipping\_field\_validation
- Fix: Fix WooCommerce translation that was misaligned with core causing the string to not be translated.
- Fix: Fix issue where a customer who downgraded their CheckoutWC license might be stuck with premium functionality turned on without anyway to turn it off.
- Fix: Fix styling issues with PayPal for WooCommerce order review screen on mobile.
- Fix: Fix issue where digital only orders could not be completed with PayPal for WooCommerce.
- Fix: Fix styling bug on review summary when order is not shipped.
- Fix: Added 'update' event from WooCommerce core to trigger update\_checkout refresh.
- Fix: Fix bug with one-time shipping and WooCommerce Subscriptions.

 **Version 3.12.2 - 2020.10.26**

- Hotfix: Fix PHP error in Admin controller from typo in function name.

 **Version 3.12.1 - 2020.10.23**

- Hotfix: Fix fatal error with WooCommerce Thank You Page - NextMove Plugin. Adds missing parameter to body\_class filter.

 **Version 3.12.0 - 2020.10.22**

 Note: This release eliminates translation of strings in the CheckoutWC admin settings screens.

- New: Click to see promo code option. Adds a link 'Have a promo code? Click here.'
- New: Tooltip on CVV fields with explanatory text for users.
- New: New 'Edit' link on cart items that appears on hover. Allows users to make larger edits to quantity of an item.
- Improved: Mobile cart summary now has a cart icon and a 'Hide order summary' link when opened.
- Improved: Added Billing Address subheading.
- Improved: Shortened Payments subheading text.
- Improved: Added class to cart items that are components of YITH Composite products for easier styling.
- Fix: Fixed issue with Elementor global styles not working on checkout page.
- Fix: Fixed styling issues with BACS gateway on thank you page.
- Fix: Fixed bug with Glass theme and Stripe for WooCommerce that caused Google Pay / Apple Pay to always be styled as selected.
- Fix: Added support for Extra Fees for WooCommerce.
- Fix: Fixed translation bug with English (UK) translations.
- Fix: Fixed bug with Checkout Add-ons select input labels not appearing.
- Fix: Fixed bug with SendCloud JS compatibility code.
- Fix: Added back AJAX output error suppression.
- Fix: Added protection to avoid fatal errors during WooCommerce upgrades.
- Fix: Fix styling for really long email addresses.
- Other: Removed translations for admin screens. This will speed up future development by eliminating 75% of the strings we have to manage with releases.
- Other: Updated tested versions to WooCommerce 4.6.1.

 **Version 3.11.1 - 2020.10.10**

- Hotfix: Fix issue where submitting checkout with PayPal for WooCommerce didn't show errors.

 **Version 3.11.0 - 2020.10.09**

- New: Support for YITH Composite Products
- Improved: Added filter for changing account creation statement: cfw\_account\_creation\_statement
- Improved: Fixed some parity issues with complete order process and WooCommerce core. Prevents payment fields from re-initing on submit error.
- Improved: Added filters for changing the size of cart thumbnails: cfw\_cart\_thumb\_width, cfw\_cart\_thumb\_height
- Fix: Fix issue with body class filter that wasn't returning classes.
- Fix: Fix error in Finnish translations.
- Fix: Fix JS error when payment field value is null. Fixes Mercado gateway.

 **Version 3.10.0 - 2020.09.30**

- New: Added Express Checkout support for Vipps
- Improved: Made it possible for developers to add additional tabs to the checkout process.
- Fix: Added margin between shipping packages.
- Fix: Added fixes fro SpaSalon theme.
- Fix: When license check fails, error is output on the screen.
- Fix: Fix issue with NIF Portugal plugin
- Fix: Fix issue with WooCommerce Square when an invalid card number is entered.
- Fix: Fix issue with PayPal for WooCommerce 2.4.0.

 **Version 3.9.3 - 2020.09.14**

- Developer: Added cfw\_after\_customer\_info\_address\_heading action
- Fix: Fix issue with caching of license activation limit that led to excessive license checks.
- Fix: Fix issue where payment request separator "Or" didn't show up with Stripe for WooCommerce.
- Fix: Added margin bottom to payment request separator.

 **Version 3.9.2 - 2020.09.10**

- Update tested versions.
- Fix: Fix error in Hungarian translations.
- Fix: Fix bug that caused Apple Pay / Google Pay to show as active on the payment gateways list with the Glass theme. (Specific to Stripe for WooCommerce - PaymentPlugins)
- Fix: Fix issue with YITH Product Bundles that caused bundled items to have editable quantities.
- Fix: Fix bug that caused return to shipping link to show up on one page checkout.

 **Version 3.9.1 - 2020.09.05**

- Fix: Fix that super annoying bug in which the phone field setting wasn't honored unless you re-saved it.
- Fix: Fix a styling issue with Stripe for WooCommerce payment express buttons.

 **Version 3.9.0 - 2020.09.01**

- New: Compatibility with themes produced by Fuel Themes. Requires latest versions.
- Improved: We now sync shipping information to hidden billing fields as they change. This is so that Jilt and similar plugins can correctly get the first and last name information.
- Improved: Refactored how we hide / show shipping tab to allow dynamically showing and hiding the shipping tab based on what the cart contains.
- Fix: Fix bug where shipping tab was not visible when using 'Hide shipping costs until calculated' option.
- Fix: Fixed a couple of PHP notices and warnings.
- Fix: Fixed bug with shipping tab when only shipped subscriptions are in the cart.
- Fix: Fixed bug with PayPal for WooCommerce not loading the email address correctly on the review page, preventing orders from being submitted.
- Fix: Fixed bug with latest version of EU VAT Number that caused field labels to not show up.
- Fix: Fix issue where (optional) might show up in promo code field.
- Fix: Fix issue with longer payment separator text on mobile devices.

 **Version 3.8.3 - 2020.08.26**

- Fix: Fixed bug where fragments from 3rd party plugins that return non-string values threw JS errors.
- Fix: Fixed bug with Germanized for WooCommerce did not pickup billing address during submit.
- Fix: Separated logic for showing shipping tab and showing shipping methods to prevent bugs from hidden shipping fields.
- Fix: Fixed Dutch translation spelling mistake.
- Fix: Fixed bug that caused 'Hide shipping costs until an address is entered' option to hide the shipping tab entirely for stores that don't have a default customer location.

 **Version 3.8.2 - 2020.08.22**

- Hotfix: Fixes critical bug that caused a license check to run on every single page view.

 **Version 3.8.1 - 2020.08.21**

- Hotfix: Fix issue with Authorize.net CIM 3.3.0. (Unrelated to 3.8.0 release)

 **Version 3.8.0 - 2020.08.21**

 **<u>CheckoutWC 3.8 requires PHP 7.0. If you upgrade on a version prior to 7.0, CheckoutWC functionality will not load.</u>**

- New: CheckoutWC now requires PHP 7.0.
- New: Settings Exporter / Importer
- New: User Matching - automatically associate guest orders with existing accounts
- New: Support for WooCommerce - Social Login (WPWeb)
- New: Support for WooCommerce MailerLite
- New: Support for Pont shipping for Woocommerce
- New: Added Arabic translations.
- Improved: Allow shortcodes in empty cart redirect URL setting.
- Improved: Dropped jQuery Migrate from script requirements.
- Improved: Checks whether any shipping packages exist when determining whether to show the shipping tab or shipping totals.
- Improved: Refactored how we fingerprint payment methods to prevent unnecessary refreshes. Now uses JS just like WooCommerce core.
- Improved: Added new filters - cfw\_ship\_to\_label, cfw\_cart\_totals\_shipping\_label, cfw\_express\_pay\_separator\_text
- Fix: Fully working Braintree for WooCommerce (PaymentPlugins) support.
- Fix: Fix issue where postal code reverted to wrong value with Square.
- Fix: Fix JS error with Ship Mondo.
- Fix: Fix issue where default WooCommerce notice wasn't styled correctly.
- Fix: Fix bug with WooCommerce style registration that caused an inconsistent state.
- Fix: Fix bug that caused enable order notes setting to become unavailable after enabling.
- Fix: Fix issue where Klarna Checkout couldn't succeed due to shipping phone field being required.

 **Version 3.7.4 - 2020.07.30**

- Developer: Added cfw\_field\_data\_persistence\_excludes filter to allow changing which fields data is persisted on refresh.
- Developer: Added cfw\_thank\_you\_title / cfw\_thank\_you\_subtitle filters.
- Developer: Added cfw\_before\_enhanced\_login\_prompt and cfw\_after\_enhanced\_login\_prompt action hooks.
- Developer: Added cfw\_breadcrumb\_cart\_url filter.
- Developer: Added cfw\_shipping\_total\_address\_required\_text and cfw\_shipping\_total\_not\_available\_text filters.
- Improved: Trim post code before validating to eliminate issues with trailing spaces.
- Improved: Don't call update\_checkout until post code field is changed instead of on key down to prevent mid entry error notices.
- Improved: Changed 'Not Calculated' notice for shipping calculation to 'Address Required' and 'Not Available' to 'No shipping methods available'
- Fix: Fix issues with SkyVerge gateways where a gateway might not set its payment fields correctly.
- Fix: Fix issue where express pay buttons didn't load properly on slow sites.
- Fix: Fix issues with latest version of EU VAT Number where VAT number field didn't show up
- Fix: Fix issue with Elementor Pro header / footer rendering behind cart summary
- Fix: Fixed issue with Salient WP Bakery plugin loading CSS that broke the checkout page layout
- Fix: Removed duplicate cfw\_after\_footer hook
- Fix: Added back "Order again" button to thank you page
- Fix: Fixed bug with Fatture in Cloud compatibility module that caused fields not to render.
- Fix: Fix potential bug with Square for slow sites where post code was not set properly.
- Fix: Fix logical error with payment gateway fingerprinting that caused payment gateways to never be refreshed on update\_checkout AJAX call.

 **Version 3.7.3 - 2020.07.09**

- Improved: Validate email field as email field even if the input type is wrong.
- Improved: Added filter to disable editable shipping phone field on order edit screen: cfw\_enable\_editable\_admin\_shipping\_phone\_field
- Fix: Fixed missing double quote in cfw\_form\_field()
- Fix: Force select labels for Checkout Add-ons select fields.
- Fix: Fix bugs with post code validation when switching countries.
- Fix: Fix bugs with Klarna Checkout
- Fix: Fix bugs with EveryPay's unique process.
- Fix: Run payment request separator handler a little later for slow loading pages.
- Fix: Fixes for Square gateway postal code field to prevent it from resetting to wrong value.
- Fix: On error during license check, report error to CheckoutWC support and delay license deactivation.
- Fix: Fix issue where header and footer were not loaded when Elementor was active, integration was enabled, but didn't have a header or footer set.

 **Version 3.7.2 - 2020.07.02**

- Fix: Fix JS errors in IE 11.
- Fix: Fix styling issues with Elementor header / footer and Glass/Copify templates
- Fix: Fix issue with Futurist breadcrumb styles
- Fix: Fix issue where Elementor being enabled could cause the header and footer not to load on the checkout page.

 **Version 3.7.1 - 2020.06.23**

- Fix: Fix issue where reload command from gateways didn't trigger a page refresh
- Fix: Fix issue where Amazon Pay endlessly refreshed
- Fix: Fix issue where placeholder for EU VAT Number filed was N/A
- Fix: Added back return to cart link on one page checkout
- Fix: Fix bug with Beaver Builder header / footer on Glass theme
- Fix: Fix issue with PayPal for WooCommerce and billing field required errors
- Fix: Fix issue where express checkout area showed up when Mollie Pay is disabled

 **Version 3.7.0 - 2020.06.19**

 This is a pretty big release in terms of the number of files changed. We obsessively tested all of the usual use cases and trouble makers and didn't identify any problems, but as always **please test thoroughly on your staging site before updating your live site** to avoid disruptions.

- NEW: Support for MolliePay through WooCommerce PensoPay
- NEW: Realtime postal code validation. If an invalid postal code is entered during checkout, an error will be immediately displayed. This does not validate that a post code is correct, just that it is a valid postal code for the selected country.
- Improved: Added JSON fixing dataFilter from WooCommerce core to complete order hook to try to cover some edge cases where servers send malformed output.
- Fix: Fix issue with WooCommerce Service forcing the shipping phone field to be optional.
- Fix: Fix issue with Braintree for WooCommerce (PaymentPlugins) PayPal button
- Fix: Fix issue where JSON output from AJAX calls encoded arrays as objects.
- Fix: Suppress express checkout separator when in final review for PayPal for WooCommerce Express Checkout orders.

 **Version 3.6.2 - 2020.06.16**

- New: When using one page checkout, cart is now position fixed so that it stays visible while scrolling.
- New: Added ability to edit the shipping phone on orders in the admin view.
- New: Added accent color option for Glass theme to control the color of the shipping options and selected accordion options.
- Improved: Shipping options, payment options, and same as shipping toggle now use pointer cursor.
- Improved: Allow individually sold products to be removed from the cart when cart editing is active
- Fix: Fix issues with Futurist breadcrumbs when skipping shipping option.
- Fix: Fix issues with Futurist theme and one page checkout.
- Fix: Fix issues with JS validation of fields when one page checkout is enabled.
- Fix: Fix issue with Authorize.net and order pay page.
- Fix: Use determine\_locale() to get the locale instead of using get\_user\_locale()

 **Version 3.6.1 - 2020.06.13**

- Hotfix: Fix issue with WooCommerce Gift Cards and the mobile coupon feature.

 **Version 3.6.0 - 2020.06.12**

 This is a pretty substantial update. There shouldn't be any breaking changes, however **please test before upgrading your live site.**

- NEW: One Page Checkout option. When enabled, the three steps become one longer step. Useful for digital stores.
- NEW: Beaver Themer support. Use Beaver Themer to build custom headers and footers and override the header and footer on the checkout page.
- NEW: Experimental Integration - Template Loader. This feature allows you to load the checkout template inside your WordPress theme. This option is unsupported, so you'll need to be prepared to deal with any styling issues that may result.
- NEW: Added support for WooCommerce Advanced Messages
- NEW: Added support for ShipIt / WooCommerce Carrier Agents
- NEW: Added support for the Tokoo theme
- NEW: Added support for the Stokie theme
- Improved: Added support for express payment buttons for Stripe for WooCommerce (PaymentPlugins)
- Fix: Fix issue with WooCommerce Order Delivery Date
- Fix: Attempt to fix issue with CSS animations and artifacts in Safari
- Fix: Fix issue with PayPal for WooCommerce smart button not displaying after toggling billing address.

 **Version 3.5.6 - 2020.06.10**

- Fix - Fix issue with invalid post code message and Square (official) gateway
- Fix - Add English (UK) translations as some people might need them.
- Fix - Add back missing order totals on order pay page.

 **Version 3.5.5 - 2020.06.09**

- Fix - Fix issue with PayPal for WooCommerce and express checkout where confirmation page didn't appear.
- Fix - Fix issue with WooCommerce Price Based on Country.
- Fix - Fix issue where currency formats that include spaces resulted in prices wrapping to the next line.

 **Version 3.5.4 - 2020.06.05**

- Fix - Fix issues with Barberry theme (specifically the Barberry Extension plugin)
- Fix - Fix issue with terms and conditions on order pay page
- Fix - Fix field layout for Brazilian Market for WooCommerce plugin
- Fix - Fix translation strings from WooCommerce core that have changed.

 **Version 3.5.3 - 2020.06.04**

- Hotfix - Fix issue with WooCommerce 4.2 that caused the row containing country, post code, and state to be invisible when either switching to a country that has no states or loading the checkout page with a country that has no states.

 **Version 3.5.1 - 2020.06.03**

- Fix - Fix issue where WooCommerce Square (official gateway) postal code field wasn't updated when the 'Same as shipping address' radio was toggled or the billing postcode was changed.
- Fix - Firm up styles on field rows to prevent themes or plugins from messing with them.
- Fix - Add more specificity to the checkmark styles on the thank you page to prevent themes or plugins from messing with them.

 **Version 3.5.0 - 2020.05.31**

 There are some pretty substantial changes here. **Please test before deploying to your live site.**

- NEW: Mobile Coupon field. Show a separate coupon field on mobile so that customers don't have to hunt for it. (Optional)
- NEW: Refactored how our tab system transitions between tabs to fix issues with gateways that use iframes. This is actually a huge performance bonus as we no longer have to selectively refresh for certain gateways like Square, Cybersource, etc.
- NEW: Support for TheBox theme.
- Improved: Added eslint and cleaned up our JS files.
- Improved: Added a new filter: cfw\_transactions\_encrypted\_statement
- Fix: Fixed issue where Authorize.net card logo watermark didn't appear.
- Fix: Fix margin on PayPal Express button.
- Fix: Fix issue where state wasn't properly filled when using Address Autocomplete.
- Fix: Fix issue with PayPalPlus and coupons.
- Fix: Fix bug with Klarna Checkout that caused an endless redirect loop.
- Fix: Fix bug with YITH Order Delivery Date.

 **Version 3.4.2 - 2020.05.22**

- Hotfix: Fix issue where Square CC fields didn't load properly.

 **Version 3.4.1 - 2020.05.22**

- Fix: Fix issue where checkout page scrolled strangely on iPhone.
- Fix: Fix issue where WP admin bar didn't position correctly on mobile devices.

 **Version 3.4.0 - 2020.05.21**

- NEW: Refactored how we refresh the checkout page to minimize the number of times it happens. This should make the checkout page much nicer to interact with and save a lot of server CPU cycles.
- NEW: Added option to skip shipping step for stores with one shipping option.
- NEW: Added support for WooCommerce Gift Cards (Official)
- Improved: We no longer block the next tab buttons during refreshes.
- Fix - Fixed bug with show mobile credit card logos option.
- Fix - Fixed bug with JupiterX theme.
- Fix - Fixed bug where opting in to stat collection double tracked stats.
- Fix - Fixed bug with NL Postcode Checker.
- Fix - Fixed bug with PostNL
- Fix - Removed warning for Checkout Field Editor for WooCommerce by ThemeHigh since customers have confirmed it works now.
- Fix - Fix styling bug with quantity steppers and IE11.
- Fix - Fix bug where clicking on promo field on phones zoomed in.
- Fix - Fix potential fatal error with Amazon Pay.
- Fix - Fix bug where save card checkbox was visible when a customer opted to not create an account.
- Fix - Fix styling bug with third party plugin checkboxes.

 **Version 3.3.0 - 2020.05.07**

- NEW: By popular request, the cart editing controls have been replaced with a quantity stepper.
- NEW: Added option to control whether thank you page template is used when viewing orders in My Account.
- NEW: Added option to show credit card logos on mobile.
- Improved: Added console logging when an unknown server response is sent during complete order.
- Improved: Added filename to downloads list.
- Improved: Moved password above create account checkbox instead of below. (Only applies option to allow customers to set a password is used)
- Fix: Fix bug where change log doesn't show up properly.
- Fix: Fix bug with newest version of Square gateway (confirmed to work with 2.1.4)
- Fix: Fix bug with YITH Order Delivery Date integration.
- Fix: Fix bug with PayPal for WooCommerce that resulted in an error about billing email being a required field.
- Fix: Fix overlay position during order submit. Now covers whole viewport and spinner will always be centered.
- Fix: Fix bug with Futurist theme and breadcrumb width on mobile.
- Fix: Fix bug where 'Allow stat collection' notice didn't actually enable stat collection.
- Fix: Fix whitespace on the right side of screen on iPhone.
- Fix: Fix issue with Braintree for WooCommerce by PaymentPlugins where error messages weren't shown.
- Fix: Fix issue where Authorize.net saved cards didn't show up properly on order pay page.
- Fix: Fix bug where conflicting styles could cause the Amazon Pay express button to have text beneath it.
- Fix: Fix bug where JS validation error messages were not translated into Greek.

 **Version 3.2.0 - 2020.05.01**

- New: Added Express checkout support for Braintree for WooCommerce by PaymentPlugins.
- New: Added support for WooCommerce Product Bundles.
- New: Greek translations.
- Improved: Added cfw\_payment\_method\_address\_review\_shipping\_method filter.
- Improved: Eliminated closures in template-hooks.php for easier unhooking.
- Improved: Added compatibility mode filter for sites that load Google Maps from another location: cfw\_google\_maps\_compatibility\_mode
- Improved: Added cfw\_cart\_item\_row\_class filter.
- Fix: Fix issues with WooCommerce style registration setup.
- Fix: Make sure cfw-customer-info-active is active on form on page load.
- Fix: Fix endless redirect bug with Klarna Checkout.
- Fix: Multiple fixes for Amazon Pay.
- Fix: Fix bug with multiple payment gateways on the order pay page, including Sezzle and PostFinance.
- Fix: Fix issue with quotes in blog name.
- Fix: Add noncing back to update checkout call. Fixes issue with plugin that expects it.

 **Version 3.1.0 - 2020.04.26**

- New: Added support for Upsell Order Bump Offer.
- New: Added official fix for Pimwick Gift Cards Pro. Adds gift card field under the coupon code field.
- Fix: Added back cfw\_after\_cart\_summary hook.

 **Version 3.0.5 - 2020.04.21**

- Fix: Fix bug with PayPal for WooCommerce and the final review screen for logged out users.
- Fix: Fix bug with latest version of Amazon Pay that caused the address fields to be hidden.
- Fix: Cleaned up locale code for field validation translations.
- Fix: Added support for getting the Weglot current locale for field validation translations.
- Fix: Fix translation of 'Contact' in Portuguese translations.

 **Version 3.0.4 - 2020.04.16**

- Improved: We now hide the WooCommerce Account setting for generating account passwords depending on your Registration Style setting.
- Improved: We now override and hide the WooCommerce Account setting for generating usernames since this should always be true for CheckoutWC.
- Fix: Fix multiple bugs with Amazon Pay.
- Fix: Fix WooCommerce warning when using Amazon Pay with PayPal for WooCommerce
- Fix: Fix potential fatal error.
- Fix: Fix bug with WooCommerce Local Pickup Plus.

 **Version 3.0.3 - 2020.04.14**

- Improved: Replace jQuery(document).ready with a lighter replacement that is more error tolerant. This makes CheckoutWC more tolerant of errors from 3rd party scripts.
- Improved: Added 67% field width option to WooCommerce Checkout Field Editor.
- Fix: Fix issue where Square gateway no loner re-ordered the payment tab to place the billing address before the credit card fields.
- Fix: Fix issue where the window did not scroll to the top properly when multiple notices were added in quick succession.

 **Version 3.0.2 - 2020.04.11**

- Fix: Fix issue where System Font Stack setting was being saved in a translated state, which broke fonts on the page.
- Fix: Fix MailChimp for WooCommerce checkbox styles.
- Fix: Fix issue where size options for WooCommerce Checkout Field Editor weren't showing up.
- Fix: Improve handling of built in form-row-first and form-row-last classes so that it uses a proper grid wrap. Fixes mobile styling of Authorize.net field gateways, etc.

 **Version 3.0.1 - 2020.04.11**

- Fix: Fix untranslated strings.
- Fix: Order admin bar menu same as the tabs in settings.
- Fix: Add updated support tab that was removed during a merge.
- Fix: Firm up background color to prevent plugins / themes from messing with it.
- Fix: Handle long label lengths for 'Ship to' in shipping address preview on shipping method and payment tabs.
- Fix: Change 'Shipping method' to 'Method' so that labels are shorter.

 **Version 3.0.0 - 2020.04.10**

 **This is a major version update. Please test before updating your live site. If you're using a custom CheckoutWC template, do NOT update. You will need to rebuild your template.**

- NEW: A brand new theme (Glass) for a brand new version (3.0!)
- NEW: Added options for the most common customizations. Control Order Notes, Cart Item options, Login and Registration right from settings.
- NEW: Reorganized admin screens to make finding things easier.
- NEW: Refactored templates to use action hooks.
- NEW: Refactored JS and CSS to be more modular and less coupled.
- NEW: Added support for Russian, Slovakian, and Japanese.
- NEW: Added support for CartFlows. You can control whether CheckoutWC loads a checkout step right from the step settings.
- NEW: More robust grid framework with better mobile responsive styles.
- NEW: Redesigned cart summary with better data display, quantity bubbles (similar to Shopify) and cart editing.
- NEW: Dynamic field resizing when switching between countries.
- NEW: Built in support for Google Fonts.
- NEW: More design options: set the body background color, text color, hover colors, and more.
- NEW: Added Shopify style preview above each step summarizing the choices made in previous steps.
- NEW: Added Weglot support.
- NEW: Support for PayPal for WooCommerce final review page.
- NEW: Option to use traditional rather than floating labels.
- NEW: When migrating your site, the stats opt-in setting will automatically turn off until you re-enable it.
- FIX: Fixed bugs with Klarna Checkout 2.x
- FIX: Fixed some Finnish translations.
- And much more! This release includes 243 commits and includes lots of little tweaks, improvements, and enhancements.

 **Version 2.44.0 - 2020.03.05**

- New: Added support for YITH Delivery Date.
- New: Added code editor to header / footer scripts and custom CSS.
- New: On activation, we now set the logo from your WordPress customizer settings if it isn't already set.
- New: Added custom text area to thank you page template. Use action: cfw\_thank\_you\_text. This renders above Order Updates.
- Improved: Better parsing of error messages that are added to the page with JavaScript.
- Improved: Added reminder when CheckoutWC is licensed and activated but not enabled.
- Improved: JS and CSS assets are now output with the version number in the filename. This busts cache automatically even when using plugins that remove version number query strings.
- Improved: Changed default colors to be more neutral.
- Fix: Fixed a few issues with Amazon Pay.
- Fix: Fixed a few issues with Genesis theme.
- Fix: Fixed a few styling issues that happen when bootstrap styles are present on the page.
- Fix: Templates now have independent webpack configs to make custom development easier. (But don't start any custom templates until version 3.0 is released!)
- Fix: Fixed bug that prevented express pay buttons from showing up if you refreshed the page on a tab other than customer information.
- Fix: Fixed bug with thank you page that prevented order status from rendering properly for unshipped orders.
- Fix: Fixed bug where Apple Pay did not show up with Stripe gateway.
- Fix: Fixed bug where New Zealand states did not populate with address autocomplete enabled.

 **Version 2.43.2 - 2020.02.17**

- Fix: Refactor how we handle showing / hiding the shipping method tab to fix issues with WooCommerce Subscriptions.
- Improved: Added alert styling to the 'There are no shipping methods available' message.
- Improved: Fixed styling issues with WooCommerce Subscription shipping methods.
- Improved: Improved how we parse error messages during checkout submit to squash some edge cases.
- Fix: Fix bug where error messages had bullet point styling.
- Fix: Fix issue with Swedish translations not working in all cases.
- Updated WooCommerce tested version to 3.9.1

 **Version 2.43.1 - 2020.02.17**

- Hotfix: Fixed express checkout wrapper showing up even when no express buttons are available.

 **Version 2.43.0 - 2020.02.14**

- New: Payment buttons now have a wrapper similar to Shopify's that says 'Express checkout': <https://www.dropbox.com/s/9s7ertyxkjnkmwc/Screenshot%202020-02-14%2016.09.54.png?dl=0>
- Improved: State dropdown now default to 'Select an option'. This is necessary because default geolocation no longer includes state.
- Improved: Added Swedish translations.
- Fix bug with Konte theme.
- Fix NextGen Gallery bug for real this time.
- Fix submit on enter bug with Safari.
- Fix overlay position bug.
- Handle custom quantities 10 and over with cart editing better.
- Switch cart list HTML to a table so we can style it more consistently.
- Fix padding on cart for Copify theme.
- Fix bug with recent versions of Checkout Add-ons.
- Fix PHP warning with constants and the Copify theme.
- Fix bug in thank you page template that didn't display the map when shipping address forced to the billing address.
- Fix bug where viewing an order that has items that no longer exists resulted in a fatal error.
- Fix styling issues with themes by hardening some of our styles.
- Fix styling bug with postal code field that caused it to appear shorter than surrounding fields.
- Fix bug where Finnish translations did not work properly.
- Fix bug with Square where error messages repeated and were unstyled.

 **Version 2.42.0 - 2020.02.08**

- New: Support for [Elementor Pro!](https://kb.checkoutwc.com/article/89-permit-elementor-styles-and-scripts-on-the-checkout-page)
- New: Support for WPC Product Bundles
- New: Compatibility with Blaszok theme
- Improved Portuguese translations.
- Improved Italian translations.
- Improved styling of cart item meta data on checkout and thank you pages.
- Workaround major bug in latest version of NextGen Gallery that prevented our AJAX hooks from returning data.
- Fix bug with placeholders and Safari credit card autocomplete.
- Fix JS errors when Google Maps script isn't loaded and autocomplete is enabled.
- Fix visual glitch with select fields that fail validation.
- Fix issue where breadcrumb tab navigation didn't show up for Copify theme on mobile.
- Fixed a PHP notice.
- Fix bug with PayPalPlusCw
- Fix issue where WooCommerce fields were being wrapped with our markup on non-checkout pages.

 **Version 2.41.3 - 2020.01.26**

- Fix issues with Portuguese and Finnish translations.
- Fix issue with NL Postcode Checker.
- Fix issue with WooCommerce 3.9 notices showing up as "Array".
- Fix issue where order pay page didn't show error message with Copify template.
- Improved: Split JS files into 2 to reduce load size of each file.

 **Version 2.41.2 - 2020.01.20**

- Fix bug with Portugal VASP Kios
- Fix bug where hidden submit button could be made visible by other plugins.

 **Version 2.41.1 - 2020.01.18**

- Updated translation files.
- Updated the way variation data is showed under cart items to better support long and complicated output.
- Fixed bug where cart is not cleared on successful order when using thank you page feature.
- Fixed bug where processing overlay / animation were not removed when checkout fails for gateways like Klarna Payments.
- Fixed bug where Polish and Portuguese translations were not loaded for some derivations of those languages.
- Fixed bug that caused gateway fields to reset when changing billing address toggle.

 **Version 2.41.0 - 2020.01.13**

- Added support for Portugal VASP Kios plugin.
- Added support for WooCommerce Advanced Shipment Tracking
- Added filter to allow overriding login failed error message: cfw\_failed\_login\_error\_message
- Prevent LastPass from monkeying around with Google API key field in settings.
- Fix issue that prevented Facebook Messenger chat from showing up.
- Fixed some PHP notices.
- Fix issue with where Jilt renders it's consent checkbox.
- Fix issue where paid to free and back switches weren't working properly.
- Fix issue with forcing WooCommerce to use billing address for billing and shipping.
- Fix issue with latest versions of PayPal for WooCommerce.
- Fix issue where register checkbox was not available when disabling the login reminder.
- Fix mobile styling issues with some payment gateways.
- Fix bug with WooFunnels Order Bump rendering the bumps twice.
- Fix bug on the thank you page that rendered the cart total on mobile instead of the order total.
- Fix styling bug on Copify theme for mobile.
- Fix bug where checkout form tries to submit when pressing enter in a field.

 **Version 2.40.2 - 2019.12.31**

- Hotfix for fatal error with some configurations that use woocommerce\_after\_shipping\_rate hook.

 **Version 2.40.0 - 2019.12.18**

 Happy Holidays! We slowed our normal release schedule to minimize problems throughout the holiday sales cycle. But we have been hard at work on a big update.

 This update includes a few refactors and while we have obsessively tested the changes, **your store is different than ours!**

 **Before updating your live site, PLEASE TEST THOROUGHLY.** We don't want any of our customers to lose sales during this important season.

- New: You can now use Checkout Field Editor to modify your billing and shipping address fields. We still think most stores should leave this alone, but this makes it much easier to add custom address fields. We also [updated our documentation](https://kb.checkoutwc.com/article/49-how-to-add-a-custom-field). This is disabled by default to prevent issues with existing stores.
- New: Added support for NIF (Num. de Contribuinte Português) for WooCommerce
- New: Added support for WooCommerce Order Delivery.
- Improved: If license is detected as inactive, we do an additional check when loading the checkout page to reduce the chance of a false positive.
- Improved: Refactored template files to use action hooks to queue the different sections. This makes it easier to maintain the template files and also makes it easier to reorder the layout of each tab without using a custom template.
- Improved: Added filters to allow tracking numbers to be added to the thank you page without using WooCommerce Shipment Tracking. Filter: cfw\_thank\_you\_tracking\_numbers
- Improved: Added better support for WooCommerce Local Pickup Plus
- Improved: Changed license check settings to not use an autoloaded WordPress option.
- Improved: Styles for 2Checkout
- Improved: Added filter to allow bypassing CheckoutWC templates. Filter: cfw\_bypass\_templates
- Improved: Order again button now appears on thank you page.
- Fixed issue where download links for digital orders did not appear on thank you page.
- Fixed issues with Amazon Pay. Create account process now works like WooCommerce native checkout.
- Fixes for issues with Amazon Pay and digital orders.
- Fixed issues with Amazon Pay and Subscription orders. When purchasing a subscription, the 'Address preview' on the shipping method tab is hidden. This is due to a currently unsolvable problem that prevents us from looking up the customers selected address accurately.
- Fixed issue with Webshipper.
- Fixed styling issues on mobile.
- Fixed issues with Hebrew language and admin settings page.
- Fixed issue with invisible checkbox fields and WooCommerce Checkout Field Editor.
- Fix - Removed #cart hash from cart link.

 **Version 2.39.3 - 2019.11.18**

- New: PayPalPlusCw gateway support.
- Improved: Added cfw\_thank\_you\_after\_cart\_summary action to thank you templates.
- Improved: Strip out some unnecessary data from update checkout, etc calls that could trigger antivirus software heuristic scanners to block dynamic updates.
- Fix: Block CSS hero from loading their CSS on the checkout page.
- Fix: Don't try to show empty WooCommerce notices.
- Fix: Fix bug with latest Avada version.
- Fix: Fix issue with Klarna Payments update.
- Fix: Fix bug where extra HTML in Copify sidebar didn't show up without special CSS.
- Fix: Thank you page now shows formatted order number instead of internal ID.

 **Version 2.39.2 - 2019.11.07**

- New: Support for Fattureincloud for WooCommerce
- Improved: Added cfw\_before\_thank\_you\_customer\_information filter and added $order object to all filters / actions on the checkout page.
- Fix: Fix issue with Avada and thank you page.
- Fix: Fix issue with Avada image lazy loading and checkout / thank you pages.

 **Version 2.39.1 - 2019.11.06**

- Improved: Made it possible to change the billing address location without breaking stuff.
- Fix: Fix issue where Oxygen Builder output conflicting styles on the checkout page.
- Fix: Fix issue where Stripe separator showed up even when no payment buttons were available.
- Fix: Fix issue where down arrow on select elements was not clickable.

 **Version 2.39.0 - 2019.11.06**

- 🎉 NEW PREMIUM FEATURE: Thank You Page - This highly requested feature allows you to replace your ugly WooCommerce thank you page with a Shopify style thank you page, complete with map embedding. [Details here.](https://kb.checkoutwc.com/article/85-how-to-enable-and-configure-the-thank-you-page)
- Improved: Added filters for every return / continue button.
- Improved: Strengthened field styles to prevent other plugins from messing with them.
- Improved: Moved all premium features to their own section in General settings.
- Fix: Fix bug with PayPal for WooCommerce final review page.
- Fix: Fix JS errors when Google maps doesn't load properly.
- Fix: Fix PHP notices.

 **Version 2.38.3 - 2019.10.26**

- Fix: Fix issues with Chronopost
- Fix: Fix issues with JupiterX theme and JupiterX Core plugin
- Improved: Added Hebrew translations

 **Version 2.38.2 - 2019.10.23**

- New: Add support for Order Delivery Date Lite.
- Improved: Alerts from pickup point shipping providers are now temporary and are removed when advancing tabs successfully.
- Fix: Fix a few asymptomatic bugs with our tabbing system after the refactor.
- Fix: Fix bug where Braintree payment fields did not load after compatibility module loader refactor.

 **Version 2.38.1 - 2019.10.21**

- Fix: Fix bug where it was impossible to go to payment when a digital product is in the cart with SendCloud and ShipMondo.
- Fix: Fix bug where JS errors happened when Klarna Checkout was activated.

 **Version 2.38.0 - 2019.10.20**

- New: Add support for Inpsyde PayPal Plus gateway.
- New: Added ability to use native WooCommerce login form with new filter: cfw\_suppress\_default\_login\_form
- New: Support for Woo Square Pro.
- New: Add ability to ask users for custom password.
- Improved: Refactored tab switching code to clean up some ugly workarounds.
- Improved: Refactored JS compatibility factory.
- Improved: Bypass flag is now comprehensive. [More info.](https://kb.checkoutwc.com/article/83-how-to-bypass-checkoutwc-for-testing)
- Fix: Fix edge case bug where PHP fatal error was possible with PayPal Checkout in one install.
- Fix: Fix translation of 'Remove Item'
- Fix: Fix deprecation warning
- Fix: Fix bug with WooCommerce 3.8.0 RC 1
- Fix: Fix ShipMondo issue with modal. Add error message to prevent going to payment without selecting pickup point.
- Fix: Fix SendCloud tab advance protection bug.
- Fix: Add translation to messages from shipping pickup point plugins that need to prevent advancing to payment before selecting a pickup point.
- Fix: Fixed breadcrumb label filter typo.
- Fix: Spinner is now centered to viewport during checkout submission.
- Fix: Fix bug with Checkout Add-ons and multi-select. All selects from Checkout Add-ons now use Select2.
- Fix: Fix bug where scroll to error messages and top of tabs did not fire.

 **Version 2.37.1 - 2019.10.05**

- Fix: Fix bug with Futurist breadcrumb.
- Fix: Fix bug where states did not populate when switching countries.
- Fix: Prevent 'undefined' text in address field when using Google Maps Address Autocomplete.
- Fix: Remove field validation errors when autocompleting state / city from post code.
- Fix: Fix issue with PixelYourSite Pro.

 **Version 2.37.0 - 2019.09.29**

- New: Support for Electro theme.
- New: In3 gateway support.
- New: WooCommerce Subscription Gifting support.
- Improved: Lots of fixes for Checkout Add-ons 2.x
- Improved: Add filters for breadcrumbs.
- Improved: Fixed issues with moving order button on order pay page for German stores.
- Fix: Catch relative protocol theme styles / scripts.
- Fix: Fix issue with low stock quantities and cart editing dropdown.
- Fix: Fix issue with add to cart notices on checkout. Added filter to conditionally show these notices when desired.
- Fix: Fix checkbox label text sizes to be more consistent.
- Fix: Style links properly according to color in settings.
- Fix: Alerts that are present on checkout page load will now persist until a subsequent update checkout AJAX call.
- Fix: SendCloud now requires picking a pickup point before advancing to the next section.
- Fix: Cleaned up some potential PHP warnings.
- Fix: Fixed bug with Order Delivery Date and PayPal Checkout that could cause an endless update loop.

 **Version 2.36.1 - 2019.09.19**

- Hotfix: The last update inadvertently applied our Avada workarounds on every page instead of the checkout page. We're really sorry about this. This update fixes the problem.

 **Version 2.36.0 - 2019.09.17**

- New: For stores that require registration, we now prevent continuing to the shipping method if we detect that your email address matches an account and that you haven't logged in.
- Improved: Allow fee only orders with order pay page.
- Improved: Switch product thumbnails to use new cfw\_cart\_thumbnail image size so that smaller images are loaded. (Requires [regeneration of thumbnails](https://www.wpbeginner.com/plugins/regenerate-thumbnails-new-image-sizes-wordpress/)to fully take advantage)
- Improved: Added more filters to allow overriding headings and label.
- Improved: When using zip autocomplete, we only fill in the city if there's only one possible match. This provides a better user experience when we can't be certain which city is the actual match.
- Improved: When using the setting 'Force shipping to the customer billing address' the address heading is now 'Billing and Shipping address'
- Fix: Fix bug with 3D Secure failures and Stripe.
- Fix: Fix bug where Avada snuck in a lot of breaking CSS.
- Fix: Fix bug where mobile total didn't update.
- Fix: Fix bug where countries that don't require postal code didn't allow continuing to next screen.
- Fix: Fix bug with Divi that hid the contents of the shipping address tab.
- Fix: Fix bug where products without inventory tracking didn't have the proper quantity options when using cart editing.
- Fix: Rollback whitespace change to totals that caused subscription prices to run continuously off of the page. If you need to prevent whitespace wrapping, you'll need to do this with custom CSS.

 **Version 2.35.0 - 2019.09.06**

- Improved: Added filter cfw\_header\_home\_url to allow changing the home URL link in the header. [More information.](https://kb.checkoutwc.com/article/80-how-to-change-the-header-link-url)
- Improved: Added the ability to adjust cart item quantity over 10. It now prompts the user to enter their desired quantity when selecting '10+'.
- Improved: Re-factored how alerts are handled to make them more consistent / standardized.
- New: Support for Flevr theme
- Fix: Fix bug where form field persistence library emptied state field on checkout submit resulting in 'Shipping/Billing State is a required field' errors

 **Version 2.34.2 - 2019.08.29**

- New: Added support for Braintree for WooCommerce: <https://wordpress.org/plugins/woo-payment-gateway/>
- Improved: Add the ability to restrict address autocomplete to specific countries: <https://kb.checkoutwc.com/article/79-how-to-add-country-restrictions-to-address-autocomplete>
- Fix: Fix bug with Smart Send
- Fix: Fix edge case bug with WP Rocket CDN settings.
- Fix: Fix login is optional translation.
- Fix: Fix styling of cart subtotal to prevent line wrap.
- Fix: Removed Amazon Pay banner from Order Pay page.
- Fix: Fix bug with Braintree and PayPal for WooCommerce.
- Fix: Fix bug with Smart Coupons send to multiple recipients option.

 **Version 2.34.1 - 2019.08.21**

- Improved: Added cfw\_show\_logout\_link filter to show the a log out link.
- Fix: Fixed issue where 'Return to cart' and 'Enter Promo Code' weren't translated.
- Fix: Fixed issue where WooCommerce German Marketplace added a fax field to the billing and shipping fields.
- Fix: Fixed issue where WooCommerce Checkout Field Editor was enforcing required states of billing / shipping address fields added prior to adding support to CheckoutWC.
- Fix: Fixed how select labels appear. They now appear at all times so that selects with empty placeholders are identifiable.

 **Version 2.34.0 - 2019.08.19**

- 🎉 NEW: Support for WooCommerce Checkout Field Editor. Due to the custom nature of our forms, we can only support **Additional Fields.** When both plugins are active, we hide the Billing and Shipping tabs from the field editor screen.
- New: Added support for Listable theme.
- Improved: Upped WooCommerce supported version to 3.7.0.
- Improved: Square Recurring Payments fields are now styled better.
- Fixed: Fixed save card checkbox styles.
- Fixed: Fix issue where Indeed Affiliates Pro broke select styles.
- Fixed: Fixed issue where Verso theme loaded search widget at the bottom of the checkout page.
- Fixed: Added back support for Square 1.x

 **Version 2.33.3 - 2019.08.09**

- Improved: Added console logging for Ajax request errors during complete order calls.
- Fix: Fix bugs with state field requirement during country switches.
- Fix: Phone field validation now matches other fields.
- Fix: Filter out empty error messages during update checkout.
- Fix: Fix potential JS errors where Square is loaded but not available due to cart conditions.
- Fix: Don't run payment gateway form fields through cfw\_form\_field.
- Fix: Styling fixes for SkyVerge payment gateway fields.

 **Version 2.33.2 - 2019.08.06**

 Minor patches for specific theme and plugin configurations. If you do not need them, you can wait to update if you prefer. All of these updates are minor and should not impact sites that do not use the affected themes or plugins.

- Fix: Patch for Verso theme.
- Fix: Patch for Optimizer theme.
- Fix: Patch for Strollik Core plugin.
- Fix: Add missing Checkout object to woocommerce\_after\_checkout\_form hook. This is needed by Klaviyo, and probably other plugins.

 **Version 2.33.1 - 2019.08.03**

- Hotfix: Fix bug where stylesheet / JavaScript assets did not load unless dev mode flag was set to true.

 **Version 2.33.0 - 2019.08.02**

- New: Added support for Atik theme.
- Improved: Get rid of Dotenv library which is unnecessary and caused issues with users who had different versions of the same library loaded.
- Improved: Move handling of woocommerce\_form\_field so that transformations apply during update\_checkout
- Fix: Fix issue with Square 2.0.
- Fix: Fix issues with Webshipper pickup points.
- Fix: Fix issue where unshipped carts calculated taxes incorrectly due to geolocation.
- Fix: Fix JS error when no payment methods are available.

 **Version 2.32.1 - 2019.07.24**

- Improved: Added warning notice in admin dashboard about incompatible plugins.
- Improved: Added filter to highlight certain countries in list of countries above the rest of the list: cfw\_highlighted\_countries
- Improved: Added filter for enabling Elementor assets (stylesheet / javascript) on the checkout page: cfw\_block\_elementor\_assets
- Improved: Added support for number fields.
- Improved: Corrected Square 2.0 credit card field styles.
- Improved: Updated translation files.
- Fix: Fix for Futurist breadcrumbs when header background color is white.
- Fix: Fix bug where active tab class was not present on initial page load.
- Fix: Fix bugs with Amazon Payments.

 **Version 2.32.0 - 2019.07.23**

- New: Support for Country Based Payments
- New: Beta support for German Marketplace
- Improved: Added cfw\_return\_to\_cart\_link\_url and cfw\_return\_to\_cart\_link\_text filters.
- Improved: Added billing and shipping level information to autocomplete attributes.
- Improved: Added cfw\_login\_optional\_text filter.
- Fix: Fix filters for changing promo code field label.

 **Version 2.31.2/2.31.3 - 2019.07.19**

- Fix: Fix fatal error for sites running &lt; PHP 7.1. Implemented automatic compatibility scanning to prevent incompatible PHP code from being released in the future.
- Fix: Fix fatal error when loading customizer.
- Fix: Fix bug where shipping method list doesn't update when applying coupons.
- Fix: Fix bug where style overrides from Design tab didn't work in production builds.

 **Version 2.31.1 - 2019.07.18**

- Hotfix: Fix fatal error on Design tab in admin settings.

 **Version 2.31.2 - 2019.07.19**

- Fix: Fix fatal error for sites running &lt; PHP 7.1. Implemented automatic compatibility scanning to prevent incompatible PHP code from being released in the future.
- Fix: Fix fatal error when loading customizer.
- Fix: Fix bug where shipping method list doesn't update when applying coupons.

 **Version 2.31.0 - 2019.07.18**

- 🍾 NEW: Added support for order-pay checkout endpoint. Disabled by default. [More information here.](https://kb.checkoutwc.com/article/75-how-to-enable-order-pay-support)
- Improved: Refactored template management and loading classes.
- Improved: Refactored zip autocomplete class.
- Improved: Added cfw\_promo\_code\_label filter.
- Improved: Added active tab class to form.
- Improved: Consolidated how notices are output on the checkout page on first load.
- Fix: Fix issue where having exactly 10 items in your cart caused the quantity dropdown to show 'Delete'.

 **Version 2.30.1 - 2019.07.17**

- Fix: Fix bug that prevented shipping address preview from updating on shipping method tab.

 **Version 2.30.0 - 2019.07.17**

 This update includes some refactoring. We tested these changes extensively and with our automated testing tools, but we cannot test every configuration. **Please make sure you test on a staging site before updating your live site.**

- Improved: Refactored totals area to use more native structure (table) for better 3rd party plugin support.
- Improved: Cleaned up Update Checkout script to use fragment approach from native WooCommerce.
- Fix: Add missing woocommerce\_checkout\_before\_order\_review / woocommerce\_checkout\_after\_order\_review hooks to Copify and Futurist templates.
- Fix: Fix issue with Checkout Add-ons outputting their fields in the wrong place.
- Fix: Fix issue with extra total row when using MyCred Partial Payments.
- Fix: Fix issue with cart editing where dynamic discounts didn't calculate properly.
- Fix: Fix issue where having more than 10 units of a cart item conflicted with cart editing.
- Fix: Fix issue with Klaviyo where carts were not tracked properly.

 **Version 2.29.1 - 2019.07.13**

- Fix: Fix styling of Stripe radio buttons.
- Fix: Don't show tax line if WooCommerce is configured to show taxes inclusively in the cart / checkout.

 **Version 2.29.0 - 2019.07.11**

- New: Added support for MyCred Partial Points as well as other plugins that use woocommerce\_checkout\_before\_order\_review / woocommerce\_checkout\_after\_order\_review hooks.
- Fix: Fix issue with Zidane theme.
- Fix: Fix issue where includes were not being loaded correctly for one site.
- Fix: Fix issue with WooCommerce Germanized that prevented Klarna Payments from working properly.
- Fix: Fix issue where removing a WooCommerce Subscription product with cart editing left the recurring totals table.

 **Version 2.28.0 - 2019.07.10**

- Improved: Checkboxes and radio buttons now use the same styling that Shopify uses.
- Improved: All fields now have a slight transition, causing the field outline and check/uncheck to animate slightly.
- Improved: When using Address Autocomplete, Address Line 1 is formatted based on the country. So for applicable countries, the address will be formatted Main St 100, instead of the US format (100 Main St)
- Improved: Fonts are now rendered with subpixel antialiasing where supported for a smoother look and feel.

 **Version 2.27.0 - 2019.07.09**

- 🎉 NEW: Address Autocomplete is here! Customers can now quickly and accurately locate their address using Google Maps. **Requires a Growth or Agency license to enable.** [More information.](https://kb.checkoutwc.com/article/72-how-to-enable-address-autocomplete)
- Fix: Fixed issue where WooCommerce Extra Checkout Fields for Brazil removed the phone fields.
- Fix: Fixed issue where Order Notes field is not displayed properly.

 **Version 2.26.1 - 2019.07.08**

- New: Added support for Divi Ultimate Header / Footer.
- Improved: Added cfw\_place\_order\_button\_container\_classes filter.
- Improved: You can now use shortcodes in footer text.
- Fix: Fixed bug with theme compatibility classes that prevented them from loading properly.
- Fix: Fixed issue where WooCommerce Germanized prevented order button from appearing.

 **Version 2.26.0 - 07/04/2019**

 Happy 4th to those of you hailing from the USA. This release has a pretty significant change regarding how fields from other plugins are rendered. As always, we recommend you test before deploying to a live site.

- New: Added filter to suppress empty cart notice after redirect when using Cart Editing: cfw\_cart\_edit\_redirect\_suppress\_notice
- Improved: All calls to woocommerce\_form\_field are now rerouted through cfw\_form\_field for styling / UI consistency.
- Improved: Consolidate support for plugins that add UI after the shipping options. Adds support for Pakettikauppa.
- Fix: Fixed bug where Braintree PayPal buttons didn't load consistently
- Fix: Added a workaround for a glitch with CO2OK and our tab system until they can fix this: <https://github.com/Mil0dV/co2ok-plugin-woocommerce/issues/32>

 **Version 2.25.0 - 07/01/2019**

- New: Added option to set the URL that checkout redirects to if the cart is emptied during cart editing.
- New: Added translations for Finland!
- New: SendCloud support!
- Improved: Added protection to prevent JS errors with Braintree.
- Improved: Hidden fields no longer get wrap containers.
- Improved: When advancing from customer information tab, all fields that have errors now highlight at the same time.
- Improved: Portuguese field validation messages now load correctly.
- Improved: Cleaned up some undefined index notices.
- Fix: Removed WOOCOMMERCE\_CART constant that was causing some issues during coupon application.
- Fix: Removed redundant cart totaling call during apply coupon action.
- Fix: Fixed Klarna Payments
- Fix: Fixed several bugs with NL Postcode Checker.
- Fix: Fixed several bugs with PostNL.
- Fix: Missing field validation translation files no longer throws a JS error.

 **Version 2.24.1 - 06/26/2019**

 Sorry for the double release. We didn't see this bug until 2.24.0 was out the door, but fortunately this was a simple fix.

- Hotfix: Fix bug where billing address overwrites shipping address.

 **Version 2.24.0 - 06/26/2019**

- 🎉 NEW: Cart editing is here! Customers can now adjust the quantity or remove cart items from checkout. **Requires a Growth or Agency license to enable.** [More information.](https://kb.checkoutwc.com/article/70-how-to-enable-cart-editing)
- Improved: Account exists AJAX call is now throttled to prevent waste of server resources.
- Fixed: Field validation messages now works with Norwegian translations.

 **Version 2.23.2 - 06/26/2019**

- Emergency Hotfix: Fix bug in 2.23.1 that allowed theme stylesheets, etc to leak into checkout page.

 **Version 2.23.1 - 06/25/2019**

- Improved: Improved Norwegian translations. Hat tip: Martin O.
- Fixed: Fixed issue where empty coupon message caused errors that break checkout.
- Fixed: Fixed issue where The7 theme compatibility fixes were applying on normal pages. This involved a slight refactor of the compatibility classes to prevent this from happening with other compatibility classes.

 **Version 2.23.0 - 06/21/2019**

- New: Added **Cart Summary Mobile Label** setting to make it easier to override the mobile cart link label. [More information.](https://kb.checkoutwc.com/article/60-how-to-change-show-order-summary-text-on-mobile-cart)
- Improved: Added preliminary support for WooCommerce Address Validation with SmartyStreets. Implementation has some glitches, but this is a start.
- Improved: Added shim for default ship\_to\_different\_address field. Before we were using this field to essentially mean the opposite of what it means on the default checkout because our address order is reversed. Now we have added an invisible shim for plugins that check this value that has a predictable, normal value and added a separate field for handling showing/hiding the billing address.
- Improved: Added cfw\_cart\_html filter to allow filtering the cart html.
- Fix: Added js-cookie to main script dependencies because some plugins expect this.
- Fix: Fixed issue with The7 theme styles leaking into checkout page.
- Fix: Fixed issue with Elementor styles messing up the checkout page.
- Fix: Fixed issue with WP admin bar display position on mobile.

 **Version 2.22.0 - 06/12/2019**

- New: Added a Recommended Plugins tab to highlight plugins that work well with CheckoutWC.
- New: Added Polish translation files.
- Improved: Mondial Relay now prevents advancing to payment method tab if pickup point is not selected.
- Improved: License key is now a password field to prevent other users from copying it (as easily)
- Improved: Refactored billing and payment radio groups to get rid of extra div wrapper.
- Improved: Phone field is now handled through native WooCommerce customizer setting. Previous CheckoutWC setting is migrated to WooCommerce setting on update.
- Fixed: Added Slovenian Parsley translations.
- Fixed: Removed PHP notice.
- Fixed: Added missing callbacks to WooCommerce action calls.

 **Version 2.21.1 - 06/04/2019**

- New: Added Square Recurring / Simple Payments For WooCommerce Subscriptions support.
- New: Added Danish translations.

 **Version 2.21.0 - 06/02/2019**

- New: Added support for Jupiter theme.
- New: Added cfw\_show\_cart\_item\_discount filter to show discount of cart items.
- New: Added support for SUMO Payment Plans.
- Improved: Added cfw\_mondial\_link\_location filter to control Mondial Relay chooser location.
- Fixed: Fixed issue where state fields would reset when clicking Complete Order button.
- Fixed: Fixed bug where selecting a country that doesn't support the city field after setting the country to a country with city fields prevented advancing to the shipping method tab.

 **Version 2.20.4 - 05/22/2019**

- New: Added cfw\_force\_display\_billing\_address which allows you to force the billing address fields to always show. (Removes the "Same as shipping address" option)
- New: Added Slovenian and Norwegian translations.
- Improved: Using cfw\_form\_field to output more fields so they show up with our styling.
- Fix: When shipping tab hidden, previous tab label had wrong tab name.
- Fix: When shipping tab hidden, validation of billing fields was sometimes incorrect.
- Fix: Fixed issue with URL used for license activation / deactivation. If you see any problems, reactivating your license should fix any issues.

 **Version 2.20.3 - 05/15/2019**

- Fix: Fixed bug that caused infinite loop when WooCommerce Subscriptions is set to not allow mixed carts.
- Improved: The fix above greatly simplifies how we identify and suppress add to cart notices when add to cart action redirects to checkout. Win win win.

 **Version 2.20.2 - 05/14/2019**

- Improved: Pass data to update\_checkout that WooCommerce passes.
- Fix: Fixed Klarna Checkout integration
- Fix: Fixed Martfury theme compatibility.
- Fix: Fixed a few glitches with Mondial Relay.
- Fix: Fixed compatibility with WPML language switcher on checkout page.

 **Version 2.20.1 - 05/10/2019**

- Improved: We found a better way to be compatible with plugins that expect the WooCommerce scripts to be loaded, allowing us to simplify a few of our compatibility classes and remove one.
- Improved: Include CSS that prevents Mondial Relay from hiding the shipping address fields.
- Fix: Fixed bug where Braintree fields reset when editing billing fields.
- Fix: Fixed an edge case bug with calculating form field rows.

 **Version 2.20.0 - 05/08/2019**

 ⚠️ If you had a problem with your license deactivating itself randomly, we are really sorry. It only affected a small number of customers, but that's no excuse!

 This release has a permanent fix, but **after you update**please go to Settings &gt; Checkout for WooCommerce &gt; License and click "Deactivate" and then "Activate" again. This will ensure you have no future problems!

- Fix: Fixed issues with PostNL
- Fix: Fixed issues with WC Postcode Checker.
- Fix: Fixed bug with EU VAT Number not removing VAT as expected.
- Fix: Fixed issues with Mondial Relay shipping provider.
- Fix: Fixed issue where cart summary background color was not respected on mobile.
- Fix: Fixed issue with inconsistent licensing URL for activations. Also ensure customers using WPML will not have issues with their license remaining active.

 **Version 2.19.1 - 05/07/2019**

- Fix: Fixed bug where 3rd party plugins calling update checkout threw a JS error.

 **Version 2.19.0 - 05/07/2019**

 This release continues to refactor the JS that runs the checkout page to make it simpler, more robust, and easier to debug. We test extensively with automated and manual tests, but as always please test before updating your live site. Your site is different than our test sites!

- New: Added support for Mondial Relay shipment provider.
- Improved: Added 3 coupon related JavaScript events: cfw-apply-coupon-success, cfw-apply-coupon-failure, cfw-apply-coupon-error, cfw-apply-coupon-complete
- Improved: Added UI blocking to dynamic areas of the checkout page. During updates, the shipping address preview, shipping methods, cart, and place order button fade out and are unclickable until the checkout is up to date.
- Improved: When a update\_checkout call errors out because the server times out, or any other reason, the blocked UI portions will unblock. This ensures users can always retry without refreshing the page.
- Improved: Ensure all update\_checkout calls use queueing system.
- Improved: Applying coupons doesn't send the shipping method. This matches core and allows for changing the selected shipping method when a coupon is applied.
- Fix: Fixed critical bug where validation script blocked checkout submit for some users.

 **Version 2.18.2 - 05/03/2019**

- Fix: Added compatibility for Atelier theme.

 **Version 2.18.1 - 05/03/2019**

- FIX: Fixed fatal error on some configurations resulting in checkout page that does not load.
- Improved: Added filter to override which URL is used for licensing checks.

 **Version 2.18.0 - 05/02/2019**

 This release contains some changes to field labels and placeholders. All optional fields now include "(optional)" at the end of the placeholder and label. This is in keeping with best practices. Also, we're using the native WooCommerce label for address\_2, so instead of the abbreviation "Apt" it's now spelled out "Apartment".

 Lastly, the address\_2 field is now full width. This mitigates some display issues on smaller screens where the label was cut off. You can always remove this field entirely by [following this guide.](https://kb.checkoutwc.com/article/64-how-to-remove-address-line-2)

- Improved: Consistently apply optional notice to all optional fields.
- Use WooCommerce native translation for most address fields.
- Fix IE11 bug that showed select dropdown for countries without states.
- Further improve cfw\_form\_field function automaticity.

 **Version 2.17.2 - 04/30/2019**

- Fix: Fixed add to cart notice suppression when redirecting to checkout with WooCommerce Direct Checkout or conventional methods.
- Also: Updated WooCommerce tested version number.

 **Version 2.17.1 - 04/29/2019**

- Oops! We left out a fix for form persistence with the state field and a label formatting fix for the Address Line 2.

 **Version 2.17.0 - 04/29/2019**

 Another release, another round of refactoring. As always, please test before deploying to your live site. We test fanatically, but we can't test every configuration.

- Improved: We're using vanilla WooCommerce localization scripts now. This sounds minor, but it was actually a pretty big refactor that fortunately allowed us to remove a lot of code that was proving to be difficult to maintain.
- Improved: Improved styling of recurring totals and before totals areas of cart summary.
- Fixed: Fixed a few Firefox styling issues related to field heights and credit card icons.

 **Version 2.16.1 - 04/26/2019**

 🚨IMPORTANT: This update includes an important fix that requires a small template change. [Please follow this guide to update your template after updating to 2.16.1.](https://kb.checkoutwc.com/article/66-upgrading-custom-templates-from-2-16-0-to-2-16-1)

- Fix: WooCommerce 3.6 made a change to how customer data is loaded on the checkout page. Our attempts to fix this in 2.16.0 caused an issue with validation that caused a small number of stores to fail checkout submission for a fresh session in an incognito window. This is fixed now and we're very sorry for any disruptions this may have caused.

 **Version 2.16.0 - 04/24/2019**

 This update has quite a few fixes in it. As always, please test before deploying to your live site. 🙏

- Add additional check to PayPal Checkout button to try to prevent double place order buttons.
- Automatic field row calculations and wraps which allows us to simplify our field API.
- Added default error when payment gateway doesn't return a reason for failure.
- Added framework for add-on settings. (Coming soon!)
- Added some additional action hooks to templates.
- Fixed German translation of phone field setting in admin.
- Fixed JS errors caused by PostNL.
- Fixed but with Martfury theme add-on plugin.
- Fixed bug with Stripe gateway Apple Pay / Google Pay buttons showing two OR dividers.
- Fixed bug where state dropdown did not repopulate correctly on refresh.
- Fixed bug with Pakkelabels modal not showing up.
- Fixed bug where selecting a shipping method caused an extra update\_checkout call.
- Prevent WC Fields Factory from messing up checkout fields.
- Added logout link for Amazon Pay and fixed layout / widget placement bugs.
- Removed some PHP notices.

 **Version 2.15.2 - 04/14/2019**

- Fixed: Braintree's hosted fields *really*don't want to load if they are not visible. To fix this, we have added a one time event that refreshes the Braintree fields after the payment tab loads. This fixes all of the issues we have been having with the fields not loading correctly.

 **Version 2.15.1 - 04/13/2019**

 Sometimes when your children keep you awake half of the night, you end up refactoring code in your head. My insomnia is your reward. 😴

- Fix: Refactored the fix for PayPal for WooCommerce billing field validation errors to be simpler and more robust. Now works for logged in users and logged out users.

 **Version 2.15.0 - 04/12/2019**

- Fix: Fixed bug where billing states did not load correctly.
- Fix: Fixed bug where PayPal for WooCommerce was unable to validate billing fields during express checkout.
- Fix: Fixed bug where Braintree credit card fields do not load.

 **Version 2.14.0 - 04/11/2019**

 This release does some minor refactoring to help broaden compatibility with other plugins. We re-tested a number of common plugins, but there's always a chance there will be an unintended side effect. **Please test yourself before updating! (Which you should always do anyway 😃)**

- Improved: Fixed bug with WooCommerce 3.6-rc2
- Improved: State label will now use the localized version such as "Region"
- Improved: State select now renders with floating label at all times, not just when you select a state.
- Improved: Added support for woocommerce\_checkout\_before|after\_customer\_details hooks from WooCommerce core.
- Improved: Added more compatibility for adding fields with woocommerce\_checkout\_fields filter.

 **Version 2.13.9 - 04/09/2019**

- Added support for WooFunnels Order Bumps.

 **Version 2.13.8 - 04/05/2019**

- New: Added support for YITH Gift Cards Premium.
- Fix: Fixed bug where Square fields don't load if it's the only gateway.

 **Version 2.13.7 - 04/03/2019**

- Improved: Move dev dependencies into require-dev and remove from release builds. Build size improved by 15%!
- Improved: Added cfw\_create\_account\_site\_name filter to modify site name in "Create % shopping account" text.

 **Version 2.13.6 - 04/02/2019**

- Hotfix: Fix translation of "Show order summary". Sorry about that!

 **Version 2.13.5 - 04/01/2019**

- New: Support for BlueCheck!
- Improved: Added cfw\_show\_order\_summary\_link\_text filter to allow "Show order summary" text to be overridden.
- Improved: Added more space for cart item prices on mobile.
- Fix: Fixed translation with NL Postcode Checker for "Street name" placeholder.
- Fix: Fixed bug where subscriptions with free trials weren't purchasable because payment fields didn't render.
- Fix: Fixed bug with Astra pro add-on.
- Fix: Fixed bug where applying 100% coupon (or otherwise making a paid order free) didn't update payment methods.

 **Version 2.13.4 - 03/29/2019**

- New: Support for Order Delivery Date
- Improved: Removed some unnecessary nonce checks.
- Fix: Fixed bug with running CheckoutWC inside a subfolder install.
- Fix: Fixed bug with NL Postcode Checker not sending an address\_1 field.

 **Version 2.13.3 - 03/27/2019**

- Fix: Fixed bug with Avada theme.
- Fix: Fixed bug with OceanWP theme and OceanWP add-ons.
- Fix: Fixed localization bug with NL Postcode Checker.
- Fix: Street name and house number now render correctly when using NL Postcode Checker or PostNL.

 **Version 2.13.2 - 03/26/2019**

- Hotfix: Fatal error that prevents summary area from loading when PayPal for WooCommerce is enabled.

 **Version 2.13.1 - 03/25/2019**

- New: Support for Savoy theme
- Improved: PostNL and NL Postcode Checker fields now render correctly without duplicated / extra fields.
- Fix: 2.13.0 added support for a WooCommerce hook that was apparently used by a number of gateways to add notices we don't want on the checkout page. We've cleaned these up on a case by case basis and the problems should be fixed.
- Fix: Fixed styling of woocommerce-error divs that were not inside our alert container.

 **Version 2.13.0 - 03/23/2019**

- New: Support for Smart Offers, Checkout Countdown Timer, and any plugin that uses woocommerce\_before\_checkout\_form
- Improved: Optimized autoloader and removed an unused PHP library
- Improved: Removed a number of compatibility classes that are no longer required. Parity FTW.✌🏻
- Fixed: Fixed bug with Square gateway where fields wouldn't render if they were not visible on page load.

 **Version 2.12.0 - 03/20/2019**

- New: YITH Points and Rewards support
- Fix: Bug with Astra theme
- Fix: Bug with PostNL 3.x

 **Version 2.11.3 - 03/19/2019**

- Improved: We now detect server errors during checkout submit, login, coupon applications, etc allowing users to have more information about what is going on with their order.
- Fix: Fixed bug preventing address line 2 label overrides from working properly.
- House keeping: Removed some vestigial logging.🧹

 **Version 2.11.2 - 03/18/2019**

- Improved: EU VAT Number now shows and hides based on the shipping country and whether or not "Same as shipping address" is checked.

 **Version 2.11.1 - 03/18/2019**

- Hotfix: Fix an issue where EU VAT Number's field was displaying twice.

 **Version 2.11.0 - 03/15/2019**

- New: Support for Smart Send
- New: Full support for Webshipper. Drop points now display underneath shipping options.
- Improved: We added a queuing system similar to WooCommerce native for update\_checkout calls. This should help slightly with performance as well as prevent tons of concurrent events.
- Improved: When PayPal Checkout is started from the cart (or product page) it will now fallback to the normal checkout page summary where the customer can simply click "Place order". We want to handle this within our template eventually, but due to complications this was the fastest path to success.
- Fixed: Fixed an edge case where one customer had a fatal error.

 **Version 2.10.2 - 03/04/2019**

- Improved: Added support for woocommerce\_cart\_item\_name filter.
- Improved: More consistently apply cfw\_checkout\_before|after\_billing|shipping\_address actions.
- Improved: Add support for woocommerce\_before\_checkout\_billing\_form, woocommerce\_after\_checkout\_billing\_form, woocommerce\_before\_checkout\_shipping\_form, woocommerce\_after\_checkout\_shipping\_form actions.
- Improved: Validate phone fields like we do other fields.
- Fixed: Bug with free orders and Stripe gateway. (Improved how we transition to free order state)

 **Version 2.10.1**

- New: Added Hungarian language translation!
- Improved: Consolidated our is\_checkout check into a single function.
- Fixed: Bug with GeneratePress theme styles on thank you page.
- Fixed: TM Organik theme includes some JS that fails on the checkout page. We worked around it.
- Fixed: Beaver Builder theme was loading some styles from its cache that affected the checkout page. It can't now!

 **Version 2.10.0**

- New: Add opt-in anonymous stat collection. Help us make CheckoutWC better!
- New: Support for YITH Deals Premium
- New: Add support for Pakkelabels
- New: Added cfw\_check\_create\_account\_by\_default filter so that you can set the default checked state of the create account checkbox. More information here: <https://kb.checkoutwc.com/article/54-how-to-set-create-account-checkbox-to-unchecked-by-default>
- New: Added support for Facebook for WooCommerce
- Improved: Detect PHP versions before 5.6 to prevent fatal error. (Plugin will activate, but not do anything - we will add a notice in a future version)
- Improved: Cleaned up translation files to remove external translation domain strings.
- Improved: It only affects us but we managed to reduce our production build process from 5 minutes to 20 seconds. And that makes us happy.
- Fix: Fixed issue with Avada theme and order received page styling.
- Fix: Shipping Phone will now show up in admin again. Also, it will continue to show up even if the phone fields are subsequently disabled.
- Fix: Prevent jQuery Touch and other libraries from messing up the mobile cart open / close functionality.

 **Version 2.9.0**

- New: Cart is now dynamically updated to support plugins like WooCommerce Price Based on Country.
- New: Added support for WooCommerce Price Based on Country.
- Fix: Prevent some WooCommerce scripts from loading at checkout that break things.
- Fix: Fixed bug with NL Postcode Checker where street address was not saved to the order.

 **Version 2.8.2**

- Fix bug with WooCommerce Germanized preventing PayPal Checkout from loading.

 **Version 2.8.1**

- Fix: Added back support for cfw\_enable\_zip\_autocomplete filter.
- Fix: Remove left over console.log
- Improved: Better handle payment gateway inits after update\_checkout called to prevent order of operations problems.

 **Version 2.8.0**

 This release includes a big change to the template form tag wrap. It *shouldn't*effect custom templates, but if you are running a custom template (and even if you aren't) **please test before updating a live site.**

- Fix: Works properly with "WooCommerce Ajax add to cart" (https://wordpress.org/plugins/woo-ajax-add-to-cart/)
- Fix: PayPal buttons now load properly on the first page load on a new session. *PayPal buttons should seriously work all the time in every situation now.*If you had asked me as a child how much of my life I expected to be consumed with figuring out why PayPal buttons don't appear, I would have cried and said "What is a PayPal button?"
- Improved: Moved form wraps so that they wrap the entire checkout page. This is necessary to allow moving the checkout button to the sidebar. More information: <https://kb.checkoutwc.com/article/37-how-to-move-the-complete-order-button-to-the-cart-summary-sidebar>

 **Version 2.7.4**

- New: Now supports gateways that dynamically update the complete order button text.
- Improved: We moved the checkout nonce field into the dynamically updated order button area. This will ensure that dynamically updated nonces get processed correctly.
- Improved: We now proactively suppress PHP warnings and notices on the checkout page, for those who have improperly configured servers.
- Improved: It hasn't come up, but we decided to proactively set cache discouraging HTTP headers on the checkout page.

 **Version 2.7.3**

- Fix PHP warning.
- Fix bug with WooCommerce Germanized where the complete order button was not rendered.

 **Version 2.7.2**

- Added a fallback method for rendering PayPal buttons. I didn't realize how much of my life would be spent asking myself the metaphysical nature of a PayPal button.
- Fix an issue where the shipping address preview didn't update on the shipping method tab.

 **Version 2.7.0/2.7.1**

 You know that episode of Breaking Bad where Walt spends an hour hunting down a fly. That's 2.7.0 and we killed the fly. We killed it good.

 There were 51 commits in this release. Please review the change log before updating, and as always **please test thoroughly before updating a live site.**

 ![](https://www.checkoutwc.com/wp-content/uploads/edd/2019/02/giphy.gif)

- New: Added support for WP Gens Refer a Friend plugin.
- New: Added preliminary support for Checkout Add-ons 2.0 (not released, keep your shirt on!)
- New: Added support for WooCommerce Social Logins (Official extension from SkyVerge)
- New: Variations that do not show up in product titles now appear in a small table underneath cart items.
- New: We now fingerprint the payment gateway markup so we can detect if a checkout update changes it. This allows us to preserve credit card fields even when the price changes.
- Improved: And because of that, we can move the billing address and checkout add-ons to the bottom of the payment tab where they naturally belong!
- Improved: Added polyfill to fix a few IE11 issues.
- Improved: Cleaned up a lot of old code from 1.x for specific gateways. We don't need it and we don't want it!
- Improved: Simplified checkout updating behaviors to reduce the number of AJAX calls. Less server load and faster UI for the win!
- Improved: Refactored zip autocomplete to run separately from validation behaviors.
- Fixed: PayPal for WooCommerce and PayPal Checkout now display their buttons properly every time!

 **Version 2.6.0**

 In 2.6.0, we continue to squash bugs and add customer requested features. Thanks for helping make CheckoutWC better. 👏🏼

- Fixed: CheckoutWC JS and CSS were loading on the order received and order pay pages. Now they aren't.
- Fixed: Payment Request Button separator wasn't loading for PayPal for WooCommerce. Now it does!
- Fixed: Sometimes the wrong PayPal button would load on checkout when using PayPal for WooCommerce. Now the right one always loads.
- Fixed: When not using smart payment buttons with PayPal Checkout, the complete order button didn't appear. Now it does!
- Fixed markup error in templates that was not causing any bugs, but was bad and now it's been banished.
- Enhancement: We added 4 new action hooks: cfw\_before\_footer, cfw\_after\_footer, cfw\_after\_cart\_summary\_totals, cfw\_after\_cart\_summary
- New: We now support EU VAT Number add-on from WooCommerce.
- New: We now support WooCommerce - Gift Cards (WP-Ronin)
- New: We now support Braintree from PayPal for WooCommerce!

 **Version 2.5.3**

 NOTE: If this is the first time you are upgrading from 2.4.x, please see the theme template note from release 2.5.0 below.

- Fix bug that prevented coupons from being applied.
- Fix how we handle jQuery as a dependency with web pack to prevent double loading jQuery.

 **Version 2.5.0/2.5.1/2.5.2**

 ⚠️ WARNING: If you are using a custom template, please [read this](https://kb.checkoutwc.com/article/32-upgrade-custom-templates-from-2-4-16-to-2-50)BEFORE upgrading. ⚠️

- Remove tests from release build to reduce size.
- Suppress add to cart notice on checkout page at all times.
- Refactor inline scripts to use wp\_localize\_script(). This should help shore up some compatibility problems with minification plugins. (Though YMMV)
- Fix bug with how billing address was handled during checkout submit.
- Fix bug with PayPal Checkout and an empty billing address at submit.
- Add support for WooCommerce Smart Coupons.
- 2.5.1: Added support for WooCommerce PostNL
- 2.5.1: Force jquery-migrate to load on checkout since some themes and plugins disable it.
- 2.5.2: Fix issue with PayPal Checkout button not showing up properly.

 **Version 2.4.16**

- Enhancement: Add support for PayPal for WooCommerce 1.5.7 (preserves legacy support for now) (Hat tip: PayPal for WooCommerce team)
- Enhancement: When switching tabs, browser will scroll to the top of the container. This is especially helpful on mobile. (Hat tip: Rafael)
- Feature: Add cursory support for Ultimate Points and Rewards. (Hat tip: Chit)
- Feature: Add support for GeneratePress Premium. (Hat tip: Chit)
- Fix: Removed PHP warning in NL Postcode Checker compatibility class. (Hat tip: Hendrik)
- Fix: Fixed issue with plugin details inheriting CFW styles in a way that broke the rendering of the native modal.

 **Version 2.4.15**

- Add support for ActiveCampaign for WooCommerce.

 **Version 2.4.14**

- Add form-row to a more logical place in the markup and use filters to move it for NL Postcode Checker.
- Add compatibility class for Porto theme to prevent it from loading stylesheets on the checkout page.
- Fix PHP syntax error in Direct Checkout compatibility class that caused issues &lt; PHP 7.x

 **Version 2.4.13**

- Add support for NL Postcode Checker.
- Add support for WooCommerce Direct Checkout.
- Fix AfterPay by Krokedil gateway.
- Improve MailChimp for WooCommerce support.
- Fix some Klarna Checkout styles.

 **Version 2.4.12**

- Fix faulty evaluation that caused a fatal error for some PayPal for WooCommerce configurations.

 **Version 2.4.11**

- Fix Klarna Checkout integration with support for fragment refresh system. Selecting Klarna from the list now performs the same action as clicking "Pay with Klarna" button.

 **Version 2.4.10**

- Add missing translation for Your Cart in Futurist theme.
- Fix bug where network activated WooCommerce was not properly detected.
- Fix field validation language library for Denmark.

 **Version 2.4.9**

- Hotfix: Removed "Unknown error" alert that was showing up briefly during successful orders for some payment gateways.

 **Version 2.4.8**

- Fix a bug that prevented Authorize.net (and possibly other gateways) from submitting properly. This was caused by our implementation of the "processing" class that WooCommerce core uses to notify gateways / plugins that it's not safe to submit. We were adding the class too early. Our sequence now matches core WooCommerce.

 **Version 2.4.7**

- Minor JS fix to logged out Amazon Pay flow.

 **Version 2.4.6**

- Improve login detection user experience: When entering an email address that is not associated with a login, the create an account checkbox will always be visible, and will default to checked. (Unless of course registration is disabled.)
- Bug: Fixed minor glitch with PayPal Checkout for WooCommerce.
- Fixed styling issue with WooCommerce Germanized.

 **Version 2.4.5**

- Fix Amazon Pay
- Fix Klarna Payments for logged in users.
- Fix how cart errors are displayed on page load.

 **Version 2.4.4**

- Improve compatibility with native WooCommerce UI blocker. (Fixes UX issue with PayPal for WooCommerce when using skip final details option)
- Don't allow themes or plugins to nuke checkout page background.
- Add separate Mexican translations with improved Spanish translations. (Props: Filiberto Flores 👍🏻)

 **Version 2.4.3**

- NEW: Payment methods and place order container are now dynamically refreshed on update\_checkout event. This more closely matches how core does their fragment updates and allows for more advanced scenarios, such as conditionally showing gateways based on other conditions.
- Fix: Fixed JS error with footer text WYSIWYG on admin screen.
- Fix: PayPal Checkout for WooCommerce now works properly.
- Enhanced: Hardened our protections against WooCommerce loading its native stylesheets and scripts on the checkout page.

 **Version 2.4.2**

- Enhanced: If shipping methods are available, show a normal shipping total instead of "Not Calculated", even when shipping hasn't been calculated.
- Enhanced: Rework theme compatibility protections for wp\_footer hook to support configurations where output buffering is disabled or not working due to other themes or plugins.
- Fix: Fix edge case JavaScript error when directly loading the shipping method tab by URL.

 **Version 2.4.1**

- Fix: Fix another issue with plugins that load old versions of Kint.
- Fix: Password placeholder is now translated properly in themes.
- Fix: CheckoutWC child templates can load their styles and scripts properly.

 **Version 2.4.0**

 **WARNING:**This release improves compatibility with other plugins, but consequently makes it more possible for themes and plugins to introduce problems. Please test and be prepared to rollback to 2.3.0 if you have significant problems. [You can download a copy of 2.3.0 here](https://www.dropbox.com/s/n19t9c3unqb3xqs/checkout-for-woocommerce-2.3.0.zip?dl=0).

- NEW: Fully working Customizer support! You can now change design settings from the front end and see what they look like in real time.
- NEW: Add support for wp\_head and wp\_footer to increase support for third party plugins!
- FIX: Google Analytics Integration now works correctly.
- FIX: Email placeholder is now properly translated.
- FIX: Address Line 2 is now properly translated.
- FIX: Amazon Pay button logo now shows up properly.
- ENHANCED: Instead of showing "Free!", shipping will now read "Not Calculated" when shipping has not been calculated and "Not Available" when no shipping methods are available.
- FIX: Fix styling of breadcrumbs on Copify template when viewing mobile styles on desktop browser.
- FIX: Fix fatal error when older version of Kint is loaded by another plugin or theme.
- NEW: Add cfw\_enable\_zip\_autocomplete filter to disable zip auto lookup. Automatically disable zip auto lookup when Checkout Address Autocomplete is activated.
- FIX: Add stricter styling to prevent gateways like Stripe from messing up our styling.
- FIX: Add compatibility class for Avada theme to prevent it from wrecking checkout page styles.
- FIX: Fixed bug where create an account checkbox could be checked and active but hidden, leading to unexpected errors.
- NEW: Added support for ToCheckoutCW, a 2Checkout gateway plugin.
- ENHANCED: Move billing address fields above payment fields so that gateways that reset on update\_checkout don't cause users to have to do double work.
- NEW: Support for Klarna Payments
- NEW: Persist payment method selection in the sessions.
- NEW: Added cfw\_checkout\_after\_payment\_tab\_billing\_address action.

 **Version 2.3.0**

- New - Added support for Klarna gateway.
- New - Added beta support for AfterPay gateway.
- Fix - Don't fire checkout\_errors JS event on success messages. This caused issues with Klarna, and possibly other gateways.
- Improved - Refactored alerts to have three flavors: warnings, errors, success
- Improved - Added email address to "Welcome back" text for logged in users.
- Improved - Login / registration settings now obey the WooCommerce -&gt; Settings -&gt; Account screen.
- Improved - Added cancel button so that users can logout of PayPal Express (with PayPal for WooCommerce - Angelleye gateway)
- Improved - Added notice after PayPal Express login so that users know to continue with checkout.

 **Version 2.2.5**

- FIX - We changed the submit button in 2.2.3 to an &lt;input&gt;, which caused some orders to double submit. This was a huge screw up and we are so sorry to anyone who installed 2.2.3 or 2.2.4 today and experienced this issue.

 **Version 2.2.4**

- Fixed - JS errors in console when registration is required.
- Improved - Added setting to General tab to enable phone fields.

 **Version 2.2.3**

- Fixed - Billing address heading no longer shows up when using Amazon Pay.
- Improved - Submit button is now a button and not a link, in case plugins or gateways expect it to be one.
- Improved - Wording for login and account creation is now simpler. Checkbox for account creation is not shown if registration is mandatory.
- Improved - Prevent conflicts between Woo Checkout Field Editor and Checkout Manager. (These plugins are still incompatible with CheckoutWC)
- Fixed - SkyVerge gateways using latest SkyVerge payment gateway framework now load their scripts properly.
- New - Added support for Cielo gateway.

 **Version 2.2.2**

- 🚨IMPORTANT FIX: WooCommerce 3.5 changed how they loaded payment gateways so that under some circumstances, gateways were not loaded before CheckoutWC's template was loaded, breaking Stripe and probably other gateways. This release fixes this issue!
- Fixed styling of Mailchimp for WooCommerce checkboxes.
- Fixed styling of paragraph tags in terms and conditions box.
- Added class "secure-notice" to all transactions are secure notice.

 **Version 2.2.1**

- Fixed bug with WooCommerce Subscriptions when only one shipping method is available.
- Fixed styling bug with Copify and Midas themes and WooCommerce Subscriptions shipping methods.
- Simplified PayPal for WooCommerce availability check to increase performance.

 **Version 2.2.0**

- Added support for Crafty Clicks.
- Added support for shipped WooCommerce Subscriptions.
- Fixed styling glitch on template settings tab.

 **Version 2.1.6**

- Add support for WooCommerce Google Analytics Integration 📈
- Add support for WooCommerce Hear About Us 🎧
- Fix bug where Stripe greedily removes separator when PayPal Express button is visible. 🐛

 **Version 2.1.5**

- Prevent plugins from re-ordering post code field in such a way that it breaks the layout.
- Add beta support for WooCommerce Germanized. Feedback welcome!

 **Version 2.1.2/2.1.3/2.1.4**

- Tweaks to Futurist theme style
- Tweak to Payment Button margins
- Tweak to Copify template top margins
- Fix breadcrumb font sizes on mobile
- Update support beacon to include documentation search and live chat

 **Version 2.1.1**

- Payment buttons are now consistently styled for Amazon Pay, PayPal Express, Payment Requests (Chrome) and Apple Pay
- Styling fixes on mobile and desktop for several of the themes.
- Fixed glitch with Login auto detection. When a user clicks the Login link, the login form will stay open even if they put in an email address that is not a valid login.
- Optimized composer autoloader

 **Version 2.1.0**

- Support for Pakkalabels for WooCommerce 📦
- Fixed bug with payment request buttons in Futurist theme. 🕷

 **Version 2.0.1/2.02**

- Fixed a bug with the logo positioning in the Futurist theme.
- Fixed bug with load order that caused filters in theme functions.php to not be used.

 **Version 2.0.0**

- 📣 Major release! There are potentially some breaking changes here, so please read the release notes thoroughly!
- 🖼 Multiple templates! In addition to the default template, we have two new templates: 
    - Copify - A theme styled to look as much like Shopify as possible.
    - Futurist - A fresh theme with a slightly different vibe.
    - Midas - The classic, default theme.

- Design settings are now specific to the template, so you can safely change templates without eliminating you current settings. 🎨
- If you have overridden the template files in your WordPress child theme, your template will still work. However it's important to update your template files as soon as possible as this functionality will be removed in a future release! ⚠
- Payment buttons like Apple Pay and Google Payment Request (both through Stripe) and PayPal Express are shown at the beginning of checkout, in a nicely formatted way that makes it easy to enable all three options. 💸
- Added support for Braintree! ⭐️
- Added support for Amazon Pay!⭐️
- Fixed compatibility issue with Pixel Your Site Pro. 🕷
- Added support for Facebook for WooCommerce. ✅
- Fixed bug with WooCommerce subscriptions.🕷

 **Version 1.6.1**

- Remove invasive styling overrides on Stripe form. Let default layout reign supreme.

 **Version 1.6.0**

- Tweak: Hide taxes from totals area when taxes are disabled.
- Fix: Change shipping address summary to use internationalized field labels.
- Added: Beta support for [PayPal for WooCommerce](https://wordpress.org/plugins/paypal-for-woocommerce/)'s PayPal gateways.
- Tweak: Imported default WooCommerce form layout styling to better support default gateway styling and removed per gateway styling for Authorize.net AIM/CIM, PayPal Express/Pro/PayFlowPro.
- Tweak: Don't use constant to pass translation domain to keep with best practices.

 **Version 1.5.7**

- Fixed bug with Chrome in Android that caused the mobile details widget to close when focusing on the promo field.

 **Version 1.5.6**

- Fix MixPanel JS output position to fix JS error.

 **Version 1.5.5**

- Add back ability to remove a coupon from checkout page.
- Add support for Portuguese language translation.
- Update debugging library Kint to 2.x to prevent conflicts with other installs.

 **Version 1.5.4**

- Added cfw\_show\_shipping\_tab filter. Allows the shipping method tab to be hidden arbitrarily by developers.
- Fixed payment icon display in recent versions of Stripe 4.1.x

 **Version 1.5.3**

- Fixed conflict between apply coupon AJAX endpoint and WooCommerce's native coupon AJAX handler.

 **Version 1.5.2**

- Add support for AutomateWoo 3.7+.

 **Version 1.5.1**

- Correct display of shipping methods when a single shipping method is available.
- Fix issue with taxes not being displayed in itemized totals.
- Added retool trigger on zip change for faster performance.

 **Version 1.5.0**

- Added support for First Data gateway: 
    - Payeezy
    - Payeezy JS
    - Global Gateway
- Improved styling of Authorize.net CIM fields
- Removed .gitignore file from output build to prevent problems with including plugin in a git repository.

 **Version 1.4.0**

- Added support for WooCommerce shipping packages.📦
- Also works with WooCommerce Advanced Shipping Packages!

 **Version 1.3.2**

- Added - Support for WooCommerce Square payment gateway.
- Added - cfw\_create\_account\_checkbox\_label filter to filter label of create account checkbox.
- Fixed - When a customer switched countries from the default country, the state was not properly sent on submit.

 **Version 1.3.1**

- Fixed bug with One Click Upsell's Stripe gateway and the compatibility module refactors.

 **Version 1.3.0**

 In no particular order:

- Refactored all compatibility classes for plugins and gateways into a new, easily maintainable structure. 🏆
- Improved Stripe gateway support robustness. 💪
- Deprecated support for Stripe 3.x. Please use Stripe 4.x.
- Fixed bug with Jilt integration not tracking recovered purchases.
- Added spinner to overlay and improved overlay display.
- Fixed bug with international addresses.
- Fixed bug with account exists AJAX check.
- Moved all AJAX endpoints to wc\_ajax from wp\_ajax. (Related to Jilt fix)
- Added support for: ✅ 
    - Google Analytics Pro
    - Enhanced Ecommerce Google Analytics for WooCommerce
    - WooCommerce Points and Rewards
    - WooCommerce One Page Checkout
    - Pixel Cat
    - AutomateWoo

 **Version 1.2.4.1**

- Hotfix to remove leftover type hints in path manager class that could cause fatal errors on activation for users in particular PHP environments.

 **Version 1.2.4**

- Fixed bug with Stripe 4.x on mobile that could prevent orders from successfully completing.

 **Version 1.2.3**

- Added support for Stripe gateway embedded in One Click Upells from WooCurve. Also supports PayPal implementation.

 **Version 1.2.2**

- Fixed edge case bug where registration password override prevented creating an account on account page. Now only applies on checkout page.

 **Version 1.2.1**

- BUG: Fix issue where "Same as Shipping" radio button resulted in billing field errors.
- BUG: Fix issue where "View cart" button could be hijacked with checkout url.
- BUG: Fix issue where JS error was possible on checkout page.
- BUG: Fix issue where billing phone was required even though phone fields were disabled.
- BUG: Fix issue where double or triple clicking submit could result in multiple orders.
- BUG: Fix issue where "Create Account" checkbox did not result in an account being created.
- ENHANCEMENT: Remove link underline on header logo area.
- FEATURE: Add support for Authorize.net CIM

 **Version 1.2.0**

- We refactored our submission model to work with more gateways out of the box. 🏗
- Stripe 4.x gateway support! (Backwards compatible with Stripe 3.x) 💳 
    - AND! Stripe Checkout (modal)
    - ALSO: Bancontact, SOFORT, Giropay, iDeal, P24, Alipay, SEPA Direct Debit, etc
- BlueSnap gateway support 💳
- Phone fields support ([added with filter](https://gist.github.com/clifgriffin/39c615e586f7e0b33eb430c56e87aab0)) 📞
- Notes field support ([added with filter](https://gist.github.com/clifgriffin/1f8f441e47ccc72675ff9cc394322b2f)) 📝

 **Version 1.1.5**

- Fixed a small bug with the add-to-cart URL parameter where normal Add to Cart requests were redirected to checkout instead of the cart. Thanks, Scott! 👏🏼

 **Version 1.1.4**

- Added support for Checkout Address Autocomplete (<https://wordpress.org/plugins/checkout-address-autocomplete-for-woocommerce/>)

 **Version 1.1.3**

- Added basic "Checkout Loads" test support for Robot Ninja ([https://robotninja.com](https://robotninja.com/))

 **Version 1.1.2**

- 🕷Fixed bug with variation combination not showing up in cart line items.
- ⭐ Added support for add-to-cart={product\_id} URL parameter. So you can pre-load the cart for checkout with a URL like: <https://demo.checkoutwc.com/checkout/?add-to-cart=56>

 **Version 1.1.1**

- Fix bug with Apple Pay separator showing up in Chrome and other browsers.

 **Version 1.1.0**

- Added support for Tickera tickets with Bridge for WooCommerce
- Added support for Redsys Gateway
- Added support for PayPal Express
- Improved styling of separator between Apple Pay / PayPal Express and customer info.
- Fix bug where checkout template overrides order-pay checkout endpoint.

 **Version 1.0.4**

- Fix internationalization issue with geolocation and state label.
- Fix safari bug on successful order.

 **Version 1.0.3**

- Fix IE 11 compatibility issues.
- Add warning for Stripe Gateway 4.x.
- Update translations.

 **Version 1.0.2**

- Add license notice to settings screen.
- Add return to cart button to customer information tab.
- Add cart breadcrumb to header links.
- Link logo to homepage.

 **Version 1.0.1**

- Fix bug where payment fields do not show up for orders that need payment.

 **Version 1.0.0**

- We have a release! 🍾🎉🙌