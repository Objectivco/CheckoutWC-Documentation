---
title: Change Log
slug: change-log
cats: Developers
status: published
---


  <p>
    <strong>Version 7.1.8 - 2022.04.18</strong>
  </p>
  <ul>
    <li>New - Added new Cart Summary Link color setting
    </li>
    <li>New - Added setting to display sale prices in cart and checkout cart summary.
    </li>
    <li>New - It is now possible to use a WooCommerce Product Bundle that contains variations as an order bump. The default variation values for each bundled product are used.&nbsp;
    </li>
    <li>Improved - Improved how product bundles are styled in the side cart and checkout cart summary
    </li>
    <li>Fix - Fix setting that appeared erroneously when side cart is disabled.
    </li>
    <li>Fix - Change label of cart item quantity color settings to add clarity to what they style.
    </li>
    <li>Fix - Fix issue where quantity stepper wasn't available in side cart unless cart editing at checkout was enabled.
    </li>
    <li>Fix - Fix issue where there were duplicate validators during checkout submission
    </li>
    <li>Fix - Attempt to fix race condition that caused the postal code validation to show an error message after correct postal code was entered
    </li>
    <li>Fix - Fix bug in admin where publishing an order bump triggered before unload alert
    </li>
    <li>Fix - Tweak our side cart coupon apply code to better match core
    </li>
  </ul>
  <p>
    <strong>Version 7.1.7 - 2022.04.14</strong>
  </p>
  <ul>
    <li>Improved - Removed some unnecessary files and compressed some others to reduce build size 30%.
    </li>
    <li>Dev - Added cfw_show_klarna_checkout_express_button filter to allow hiding Klarna Checkout express button.
    </li>
    <li>Fix - Don't allow quantity of order bumps to be changed.
    </li>
    <li>Fix - Fix issue where elements of checkout page were unblocked during an update.
    </li>
    <li>Fix - Fix WooCommerce Gift Cards field in Cart Summary sidebar.
    </li>
    <li>Fix - Get rid of duplicative events that caused multiple calls to zip code autocomplete API.
    </li>
    <li>Fix - Fix issue with express checkout buttons being hidden that were active.
    </li>
    <li>Fix - Fix issue with Checkout Field Editor that caused 50% width fields to be rendered incorrectly.
    </li>
    <li>Fix - Fix issue that caused address field changes to apply on my account page.
    </li>
    <li>Fix - Allow country field to be removed with Checkout Field Editor without causing postal code validation errors.
    </li>
    <li>Fix - Fix JS error with Braintree for WooCommerce (Payment Plugins) gateway.
    </li>
  </ul>
  <p>
    <strong>Version 7.1.6 - 2022.04.09&nbsp;</strong>
  </p>
  <ul>
    <li>Fix - Override Braintree for WooCommerce Google Pay button fill mode.
    </li>
    <li>Fix - Change how we handle empty Braintree for WooCommerce to be a bit safer.
    </li>
  </ul>
  <p>
    <strong>Version 7.1.5 - 2022.04.08</strong>
  </p>
  <ul>
    <li>New - Added setting to show Side Cart continue shopping button
    </li>
    <li>Dev - Added cfw_before_side_cart_totals action
    </li>
    <li>Dev - Added cfw_disable_side_cart_auto_open filter
    </li>
    <li>Dev - Added cfw_login_modal_last_password_link filter
    </li>
    <li>Fix - Fix logic for check create account checkbox by default setting
    </li>
    <li>Fix - Fix potential PHP warnings
    </li>
    <li>Fix - Fix styling of promo code when normal/non-floating labels are enabled
    </li>
    <li>Fix - Fix styling of lost password link
    </li>
    <li>Fix - Fix bug that caused continue shopping button to appear at the bottom of regular thank you page template
    </li>
    <li>Fix - Fix bug where logo was not visible using Klarna Checkout with the Copify theme
    </li>
    <li>Fix - Prevent account user name from sneaking into the account fields at checkout
    </li>
    <li>Fix - Non-floating labels can now wrap to the next line
    </li>
    <li>Fix - Fix issue where uninitiated Braintree for WooCommerce payment request buttons such as Apple Pay still showed up when not available
    </li>
  </ul>
  <p>
    <strong>Version 7.1.4 - 2022.04.03</strong>
  </p>
  <ul>
    <li>Fix - Fix potential infinite loop that caused update_checkout to run continuously when WooCommerce German Market was active. Fixes other potential scenarios that would cause the same thing
    </li>
    <li>Fix - Fix styling glitch where loading shimmer didn't fully cover payment gateway titles.
    </li>
  </ul>
  <p>
    <strong>Version 7.1.3 - 2022.04.01</strong>
  </p>
  <ul>
    <li>New - Added new option to place Trust Badges in the footer. Trust Badges now have a main level admin menu.
    </li>
    <li>Improved - The official Stripe gateway undeprecated an important filter that allows us to turn on payment request/express buttons on the checkout page. So we re-implemented it.
    </li>
    <li>Improved - The whole row is now clickable to select a payment method. Particularly helpful on the Glass theme due to the larger styling of items.
    </li>
    <li>Dev - Removed cfw_disable_admin_menus filter in favor of better methods. &nbsp;Try: remove_menu_page( 'cfw-settings' )
    </li>
    <li>Dev - Added new action: cfw_order_item_after_data
    </li>
    <li>Fix - Fix issue where Full Name, House Number, and Street Name fields caused issues with express checkout (Apple Pay, Google Pay, etc)
    </li>
    <li>Fix - Corrected some Danish translations. Thanks, Julie!
    </li>
    <li>Fix - Fix how we style the footer on the Glass theme. No longer uses absolute positioning which I think we can all agree is better.
    </li>
    <li>Fix - Fix bug that caused countries that are excluded in WooCommerce settings to show up in international phone field dropdown.
    </li>
    <li>Fix - Revert changes to Netherlands zip autocomplete in favor of disabling zip autocomplete entirely for the Netherlands and Belgium due to our data source not having good city data.
    </li>
    <li>Fix - Fix edge case where if a shipping address field value was 'null' the billing address sync would still run.
    </li>
    <li>Tweak - Removed colon after shipping method names
    </li>
    <li>Tweak - Renamed pot file to checkout-wc.pot since this seems to be more standards complaint.
    </li>
  </ul>
  <p>
    <strong>Version 7.1.2 - 2022.03.30</strong>
  </p>
  <ul>
    <li>Fix - Fix issue with header bottom margin when header background color is white
    </li>
    <li>Fix - More strenuously protect from fatal errors in PayPal for WooCommerce compatibility class.
    </li>
    <li>Fix - Don't require full name, street name, or house number fields during payment requests from Stripe, WooCommerce Payments, Square, or Klarna Checkout.
    </li>
    <li>Fix - Fix another issue with the word optional not being translated properly&nbsp;
    </li>
    <li>Fix - Fix some Danish translations
    </li>
  </ul>
  <p>
    <strong>Version 7.1.1 - 2022.03.25</strong>
  </p>
  <ul>
    <li>Fix - Fix fatal error in PayPal for WooCommerce compatibility class
    </li>
  </ul>
  <p>
    <strong>Version 7.1.0 - 2022.03.25</strong>
  </p>
  <ul>
    <li>New - You can now elect to display trust badges below the checkout form in a horizontal row.
    </li>
    <li>New - Added loading animation on continue buttons at the bottom of each step that runs while asynchronous field validation is running.
    </li>
    <li>Improved - Use native form-row class as parent styling class instead of cfw-input-wrap. Makes it easier to style fields without fulling controlling every aspect of the field output.
    </li>
    <li>Improved - Added list of common email address domains that short circuit domain check resulting in faster validation.
    </li>
    <li>Improved - Fields that are not visible on the active tab are no longer validated. Also added a lot more logging when using cfw-debug=true URL parameter to identify which field is causing validation failures.
    </li>
    <li>Fix - Fix bug that caused the footer text color option to not work.
    </li>
    <li>Fix - Fix bug that caused Order Bumps admin menu to show for non-admins.
    </li>
    <li>Fix - Fix bug that caused the Show Credit Card Logos on Mobile option to not work on the Order Pay page.
    </li>
    <li>Fix - Fix multiple bugs that prevented order submission when using PayPal for WooCommerce and our full name field as well as our discreet address 1 fields.
    </li>
    <li>Fix - Billing address sync was trying to sync non-address shipping fields such as shipping methods.
    </li>
    <li>Fix - Fix issue with autocompleting city from zip for Dutch addresses.
    </li>
    <li>Fix - Fix issue with (optional) not being translated in field placeholders and on Add Address Line 2 type links.
    </li>
    <li>Fix - Fix validation errors with Iconic Delivery Slots when their UI was not visible
    </li>
    <li>Fix - Fix bug where HTML was added to field placeholders from label
    </li>
    <li>Fix - Styling improvements for Order Delivery Date Pro
    </li>
    <li>Fix - Fix edge case bug where missing trust badges data caused a fatal error.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.16 - 2022.03.18</strong>
  </p>
  <ul>
    <li>Fix - Fix styling of WooCommerce Checkout Add-ons fields
    </li>
  </ul>
  <p>
    <strong>Version 7.0.15 - 2022.03.17</strong>
  </p>
  <ul>
    <li>Fix - Fix directions for activating CheckoutWC templates.
    </li>
    <li>Fix - Suppress validation during Amazon Pay using a different method.
    </li>
    <li>Fix - Use more accurate way of getting element height when detecting payment request (express checkout) buttons
    </li>
    <li>Fix - Fix bug that could cause update_checkout to run in an infinite loop when address fields are mismatched
    </li>
  </ul>
  <p>
    <strong>Version 7.0.14 - 2022.03.16</strong>
  </p>
  <ul>
    <li>WooCommerce Wholesale Lead Capture is hijacking all hidden fields and replacing the value with the placeholder which is breaking how we store the email address for logged in users. Because a lot of our customers seem to use this plugin we have changed how we output the hidden field and no longer use woocommerce_form_field() to output it and instead just directly print a hidden field.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.13 - 2022.03.13</strong>
  </p>
  <ul>
    <li>Fix - Fix bug where 'shim' country showed up when only one shipping or billing country was defined. This effectively reverts "Fix - Don't let themes and plugins mess with field markup" We'll let themes and plugins make these modifications for now and deal with them as they arrive.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 7.0.12 - 2022.03.11</strong>
  </p>
  <ul>
    <li>Fix - Fix bug with preventing form field changes on non-checkout pages that impacted the Side Cart when the promo field was enabled.
    </li>
    <li>Fix - Fix styling bug with Flatsome and the quantity plus button in the side cart / checkout.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.11 - 2022.03.11</strong>
  </p>
  <ul>
    <li>Fix - Fix bug with how we prevented other themes and plugins from messing with field markup that caused some of our own functionality to get disabled
    </li>
    <li>Fix - Prevent our form field changes from applying on non-checkout related pages
    </li>
  </ul>
  <p>
    <strong>Version 7.0.10 - 2022.03.11</strong>
  </p>
  <ul>
    <li>Fix - Don't allow field labels to wrap
    </li>
    <li>Fix - Don't let themes and plugins mess with field markup
    </li>
    <li>Fix - Prevent Avada inline CSS on the checkout page
    </li>
    <li>Fix - Chrome Autocomplete Bug fix JS was running a bit greedily
    </li>
    <li>Fix - Fix conflict between WooCommerce Germanized, CheckoutWC, and WooCommerce PayPal Payments
    </li>
    <li>Fix - Fix issue that prevented account password from focusing on login modal open
    </li>
  </ul>
  <p>
    <strong>Version 7.0.9 - 2022.03.10</strong>
  </p>
  <ul>
    <li>New - Added preliminary support for WooCommerce EU/UK VAT Compliance Premium
    </li>
    <li>New - Added support for WooCommerce Tipping
    </li>
    <li>New - Added ability to determine what happens to an Order Bump when it no longer is valid. You can now opt to leave it in the cart but remove the discounts (how it worked previously) or remove the bump from the cart entirely.
    </li>
    <li>Improved - The floating Side Cart button is now hidden on the cart page.
    </li>
    <li>Fix - Fix errant display of customer information step navigation when one page checkout enabled.
    </li>
    <li>Fix - Fix bug where 'Add Address Line 2' style optional field links were rendered on account page.
    </li>
    <li>Fix - Added a delay to focusing password field when login modal opens to try to help it work more often.
    </li>
    <li>Fix - Fix how we prevent the page from scrolling when side cart is open so that layout of the page is not affected.
    </li>
    <li>Fix - Fix styling glitch on small screens with shipping method titles wrapping beneath radio buttons.
    </li>
    <li>Fix - Fix bug with 'Change' link in preview area on small screens. Prevents text wrapping.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.8 - 2022.03.09</strong>
  </p>
  <ul>
    <li>Fix - Fix issue where billing address wasn't synced from shipping address when logging into PayPal Express through Payment Plugins Braintree for WooCommerce express button.
    </li>
    <li>Development - Stopped listening for esoteric events like cfw_address_autocompleted and instead pass it as a parameter.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.7 - 2022.03.09</strong>
  </p>
  <ul>
    <li>Fix - Fix potential fatal error if field class argument isn't set.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.6 - 2022.03.09</strong>
  </p>
  <ul>
    <li>Improved - Password field will now be focused if username field has value when login modal opens.
    </li>
    <li>Improved - Added new action: cfw_after_side_cart_proceed_to_checkout_button
    </li>
    <li>Improved - Page will no longer scroll when side cart is open.
    </li>
    <li>Fix - Fix bug that caused upload logo button to fail.
    </li>
    <li>Fix - Fix Amazon Pay bugs that made it impossible to finish checkout.
    </li>
    <li>Fix - Fix regression that caused Garlic to overwrite session field values.
    </li>
    <li>Fix - Catch error with intl-tel-input when country is not in their list.
    </li>
    <li>Fix - Fix bug that caused first and last name values to be cleared on page load.
    </li>
    <li>Fix - Fix styling of adhoc notices from Payment Plugins Stripe for WooCommerce and the Copify / Glass themes
    </li>
    <li>Fix - Fix bug that prevented WooCommerce Conditional Shipping and Payments to not show their notices correctly.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.5 - 2022.03.08</strong>
  </p>
  <ul>
    <li>Fix - Fix errant translation for 'Full name' in British English translations.
    </li>
    <li>Fix - Fix uncaught exception when Google Maps fails to load.
    </li>
    <li>Fix - Add back Continue Shopping button to side cart behind this filter: cfw_side_cart_enable_continue_shopping_button. Disabled by default.
    </li>
    <li>Fix - Revert changes that removed error logging from update checkout AJAX refresh.
    </li>
    <li>Fix - Fix bug that caused the Full Name field to show an error on page load.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.4 - 2022.03.07</strong>
  </p>
  <p>
    Hotfix for 7.0.0. <strong>&nbsp;</strong><em>Read the 7.0&nbsp;release notes below!</em>
  </p>
  <ul>
    <li>Fix - Fix bug where login modal wasn't pre-filled with email address.
    </li>
    <li>Fix - Fix bug where registration setting in CheckoutWC &gt; Checkout was applied inconsistently.
    </li>
    <li>Fix - Fix translation domain of "It looks like you already have an account" phrase in login modal.
    </li>
    <li>Fix - Fix bug where billing address wasn't synced from shipping address on zip autocomplete.
    </li>
    <li>Fix - Fix bug where phone field validation messages were shown when phone field was not required when using International Phone Field feature.
    </li>
    <li>Fix - Fix bug with Trust Badges admin that caused all images to be replaced when uploading an image to a new trust badge.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.3 - 2022.03.07</strong>
  </p>
  <p>
    Hotfix for 7.0.0. <strong>&nbsp;</strong><em>Read the 7.0&nbsp;release notes below!</em>
  </p>
  <ul>
    <li>Fix - Fix potential fatal error on Thank You page admin settings page.&nbsp;
    </li>
    <li>Fix - Fix styling of shipping method prices. Price now aligns to the right correctly.
    </li>
    <li>Fix - Fix margin between coupon code field and apply coupon button on mobile.
    </li>
    <li>Fix - Fix bug that caused Zimbabwe to be selected on page load.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.2 - 2022.03.07</strong>
  </p>
  <p>
    Hotfix for 7.0.0. <strong>&nbsp;</strong><em>Read the 7.0&nbsp;release notes below!</em>
  </p>
  <ul>
    <li>Fix - Fix bug that caused fatal error when viewing drafts in WP admin.
    </li>
    <li>Fix - Fix bug that caused the shipping step to show when it was disabled.
    </li>
    <li>Fix - Remove left over debugging console.log&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 7.0.1 - 2022.03.06</strong>
  </p>
  <p>
    Hotfix for 7.0.0. <strong>&nbsp;</strong><em>Read the 7.0&nbsp;release notes below!</em>
  </p>
  <ul>
    <li>Fix - Fix bug with stores that only ship to one country that caused the country to be rendered in an ugly fashion.
    </li>
    <li>Fix - Fix bug that occurred when highlighted countries weren't in countries list.
    </li>
    <li>Fix - Fix bug with Custom CSS setting that caused it not to be output correctly.
    </li>
  </ul>
  <p>
    <strong>Version 7.0.0 - 2022.03.05</strong>
  </p>
  <p>
    Important: This is a MAJOR release. Please use caution when updating. There were over 360 code changes in this release with some substantial changes to underlying functionality.&nbsp;
  </p>
  <p>
    This release removes a number of hooks and filters that are no longer needed but could impact your site if you or your developer wrote custom code to modify your CheckoutWC pages. Before updating, please confirm that you aren't using <a href="https://www.checkoutwc.com/documentation/removed-action-hooks-and-filters-in-7-0">any of these actions or filters in your custom code</a>. (Most likely you aren't using these hooks, but please check first.)
  </p>
  <p>
    <em>Please backup your site before updating and test on a staging site first BEFORE updating your live site.</em>
  </p>
  <ul>
    <li>New - Redesigned login flow to use modal instead of the password slide down. Customers were sometimes confused by the current login process because the email field was also functionally a username field for the purposes of logging in, and sometimes the password field was for setting a new password and sometimes it was for logging in. The new flow makes these discreet steps that can't be confused for one another.
    </li>
    <li>New - Redesign quantity control for Cart Editing At Checkout as well as Side Cart. Buttons are bigger and easier to use on mobile devices as they are more accessible.
    </li>
    <li>New - Fields are now rendered with the native woocommerce_form_field() function with some of our own secret sauce to tweak the output for styling purposes.
    </li>
    <li>New - Added inline email domain validation. Email addresses with invalid domains (domains without MX records) are now rejected.
    </li>
    <li>New - Added inline post code validation. Errors regarding postcodes are now shown under the post code field like other validation errors.
    </li>
    <li>New - Refactored how tabs are output and how they are validated to make them more composable. It is now much easier to add a custom tab.
    </li>
    <li>New - Completely redesigned and reorganized admin pages. We hope you love them!
    </li>
    <li>New - It's now possible to indicate the quantity of product added to the cart when an Order Bump is accepted.
    </li>
    <li>New - Optional fields are now hidden until link is clicked. Example: Add Address Line 2 (You can turn this off in settings)
    </li>
    <li>New - Discreet Address 1 Fields. You can now opt to use separate House Number and Street Name fields. Helpful for our European friends.
    </li>
    <li>New - Full Name field. Show one full name field instead of first and last name fields. Optional.
    </li>
    <li>New - You can now preview different templates without switching templates.
    </li>
    <li>New - You can now define separate header / footer scripts per page (Checkout, Order Pay, Thank You)
    </li>
    <li>New - User Matching, Order Review Step, One Page Checkout, and Php Snippets are now available to all license holders.
    </li>
    <li>Improved - Refactored alerts/notices. Gateway notices now appear next to gateway fields as designed. Scrolling to the top for other notices is now smoother and doesn't lockup the browser.
    </li>
    <li>Improved - Removed calls to deprecated jQuery functions.
    </li>
    <li>Improved - Implement native browser hash change support in tab system.&nbsp;
    </li>
    <li>Improved - Change how we hook empty Side Cart message to make it more easily customizable by devs like you
    </li>
    <li>Improved - We now suppress WP emojis script from loading on checkout page.
    </li>
    <li>Fix - Fix bug where some express buttons didn't get the loading shimmer animation.
    </li>
    <li>Fix - Fix visual glitch with loading shimmer and order pay page buttons.
    </li>
    <li>Fix - Fix bug that caused coupon alerts to persist between attempts to apply a coupon code.
    </li>
    <li>Fix - Fix visual bug with coupon code field styling.
    </li>
    <li>Fix - Fix styling bugs with international phone field.
    </li>
    <li>Fix - Fix bug where changing the email field caused a refresh when using One Page Checkout, which is unnecessary.&nbsp;
    </li>
    <li>Fix - Allow HTML in notices / alerts.
    </li>
    <li>Fix - Fix errors in Finnish translations.
    </li>
    <li>Fix - Fix bug with express buttons area showing up when there are no express buttons.
    </li>
    <li>Fix - Fix visual glitch on page load that caused all tabs to be briefly visible.
    </li>
    <li>Fix - Fix issue that caused the first tab to load when linking to a URL with a different tab. It is now possible to link directly to a specific step (as long as the previous steps have been completed)
    </li>
    <li>Fix - Fix bug where SmartyStreets modal tried to open twice, making it impossible to close it.
    </li>
    <li>Fix - Fix bug where SmartyStreets could effectively bypass other validation.
    </li>
    <li>Fix - Fix bug that caused shipping email field to not render for WooCommerce Pakettikauppa plugin
    </li>
    <li>Fix - Fix bug with SmartyStreets that caused the wrong country to be returned.
    </li>
    <li>Fix - Fix bug that caused an abbreviated city name to be set when using Google Address Autocomplete.
    </li>
  </ul>
  <p>
    <strong>Version 6.2.4 - 2022.02.11</strong>
  </p>
  <ul>
    <li>Fix - Fix JS error when country field is not present.
    </li>
    <li>Fix - Fix issue &nbsp;with payment gateway change handlers that was causing an infinite AJAX refresh
    </li>
    <li>Fix - Fix fatal error caused by calling non-static method statically.
    </li>
    <li>Fix - Fix potential fatal error with Klarna Payments.
    </li>
    <li>Fix - Order failed text is now on the thank you page where it always should have been for those odd situations where a gateway sends someone to the order-received endpoint with a failed order.
    </li>
    <li>Fix - Fix improper detection of whether the selected payment gateway changed.
    </li>
    <li>Fix - Post code field no longer fires AJAX refresh on keydown to prevent poor UX with improper post code detection
    </li>
    <li>Improved - Refactored Google Address Autocomplete functionality to better handle different completion strategies for different countries.
    </li>
    <li>Development - Added unit testing for Google Address Autocomplete.
    </li>
  </ul>
  <p>
    <strong>Version 6.2.3 - 2022.01.14</strong>
  </p>
  <p>
    We have a lot of stuff in the works, but today we're releasing a tasty patch release that fixes some bugs and generally makes CheckoutWC better for everyone.
  </p>
  <ul>
    <li>New - Add support for YITH Points and Rewards 3.x
    </li>
    <li>Improved - Automatically exclude our JS files from WP Rocket transformations that break things.
    </li>
    <li>Improved - Added action before upsells are added to the cart: cfw_before_order_bump_add_to_cart
    </li>
    <li>Improved - When rendering a remove item link, we now pass it through the WooCommerce filter so that it picks up changes from other code.
    </li>
    <li>Improved - Refactored Google Address Autocomplete service. It's cleaner! It's faster! (maybe) And it's much easier to handle country by country edge cases.
    </li>
    <li>Fix - Fix multiple bugs with Checkout Field Editor (official WooCommerce extension)
    </li>
    <li>Fix - Clean up jQuery migrate warnings.
    </li>
    <li>Fix - Fixes for PayPal for WooCommerce Complete Payments gateway.
    </li>
    <li>Fix - Fix bug where error messages were not properly displayed if the error was not output in the form tag.
    </li>
    <li>Fix - Fix bugs with Thrive theme.
    </li>
    <li>Fix - Aborted AJAX calls are no longer logged as errors.
    </li>
    <li>Fix - Eliminated deprecated function call.
    </li>
    <li>Fix - Fix bug with Metro theme.
    </li>
    <li>Fix - Fixed bug where upsells were not discounted properly after being added to the cart.
    </li>
    <li>Fix - Fix bug where the city field was not validated if it was rendered off screen.
    </li>
  </ul>
  <p>
    <strong>Version 6.2.2 - 2021.12.18</strong>
  </p>
  <p>
    <strong>'Tis the season to be conservative about plugin updates!&nbsp;</strong>ðŸŽ„&nbsp;If your store is humming along through the holiday rush,&nbsp;<em>you may want to wait a few weeks on this update.</em>&nbsp;But if you like the gifts below, receive them with our blessing. (After careful testing!)
  </p>
  <ul>
    <li>Fix - Fix potential fatal error with EU VAT Assistant compatibility module.
    </li>
    <li>Fix - Reworked order review step to hopefully allow it to work with more gateways.
    </li>
    <li>Fix - Fix JS error when address autocomplete is enabled but there are no address fields.
    </li>
    <li>Fix - Debounce scrolling to alerts.
    </li>
    <li>Improved - Refactored AJAX actions to use super.error() method and cleaned up unused properties/getters/setters.
    </li>
  </ul>
  <p>
    <strong>Version 6.2.0/6.2.1 - 2021.12.13</strong>
  </p>
  <p>
    <strong>'Tis the season to be conservative about plugin updates!&nbsp;</strong>ðŸŽ„&nbsp;If your store is humming along through the holiday rush,&nbsp;<em>you may want to wait a few weeks on this update.</em>&nbsp;But if you like the gifts below, receive them with our blessing. (After careful testing!)
  </p>
  <ul>
    <li>Improved - Refactored Order Bumps to distinguish between different types of bumps and separate their logic.
    </li>
    <li>Improved - For products visible in the catalog, clicking an order bump's thumbnail will open the product page in a new window.
    </li>
    <li>Improved - Added a new function for grabbing all order bumps: cfw_get_all_order_bumps
    </li>
    <li>Improved - Added some unit tests to FormAugmenter
    </li>
    <li>Improved - Added unit testing to stat collection classes
    </li>
    <li>Improved - Added unit test to YITH Composite Products compatibility module
    </li>
    <li>Improved - If update_checkout AJAX call fails, display a message letting customers know but return UI to normal state.
    </li>
    <li>Improved - If update_checkout AJAX call fails, still trigger payment gateway init and updated_checkout JS event like WooCommerce core does.
    </li>
    <li>Improved - If an error notice is already on the page and the same notice is on the next request, briefly animate the error notice with a shaking effect so that customers realize the error still applies.
    </li>
    <li>Fix - Fix a loophole that allowed people to get order bump special pricing without qualifying for the bump.
    </li>
    <li>Fix - SmartyStreets now works when shipping address is forced to billing address.
    </li>
    <li>Fix - Implemented automatic LTR &gt; RTL CSS conversion.
    </li>
    <li>Fix - Adjust priority of our assets to avoid a conflict with Divi.
    </li>
    <li>Fix - Significant fixes for WP Rocket's handling of WooCommerce fragments and how this affects Side Cart.
    </li>
    <li>Fix - Similarly, we made sure side cart works with the popular plugin Disable Cart Fragments.
    </li>
    <li>Fix - If an order bump's offer product is on sale, that price is used as the base price for any bump specific discounting.
    </li>
    <li>Fix - Fix bug with Free Gifts for WooCommerce that caused the Side Cart not to open when quantity triggered free gift.
    </li>
    <li>Fix - Fixes for Order Delivery Date plugin.
    </li>
    <li>Fix - Fix for EU VAT Assistant and digital only orders.
    </li>
    <li>Fix - Fix bug that prevented order stats from being collected for many sites.&nbsp;
    </li>
    <li>Fix - Fix bug with WooFunnels Order Bump Upsells that caused AJAX update loop
    </li>
    <li>Fix - When upgrading CheckoutWC, clear WP Rocket's fragment cache
    </li>
    <li>Fix - Fix bugs in how cart item data was displayed, particularly with WooCommerce Product Add-ons
    </li>
    <li>Fix - Fix bug where quantity of side cart button did not update when cart updated.
    </li>
    <li>Fix - Fix potential error if first gateway in session is null
    </li>
    <li>Fix - Fix bug with WooCommerce Memberships that caused AJAX calls to fail when restriction mode was set to redirect.
    </li>
  </ul>
  <p>
    <strong>Version 6.1.7 - 2021.11.19</strong>
  </p>
  <ul>
    <li>New - Added support for Free Gifts for WooCommerce&nbsp;
    </li>
    <li>Improved - Added missing woocommerce_before_thankyou hook
    </li>
    <li>Improved - Exclude our JS and CSS from WP Rocket optimizations automatically
    </li>
    <li>Improved - Refactored cfw_form_attributes() and added a new filter for adding your own attributes: cfw_form_attributes
    </li>
    <li>Fix - Fix bug where invalid post codes did not generate an error message
    </li>
    <li>Fix - Fix bug where null cart item data was still displayed on checkout page.
    </li>
    <li>Fix - Fix bugs with UK addresses and SmartyStreets
    </li>
  </ul>
  <p>
    <strong>Version 6.1.6 - 2021.11.10</strong>
  </p>
  <ul>
    <li>New - Added preliminary support for WooCommerce EU VAT Assistant.
    </li>
    <li>Fix - Fix bug with method that determines if all shipping packages have a selected shipping method
    </li>
    <li>Fix - Regenerated stale MO files for de_DE and de_DE_formal translations.&nbsp;<em>Der Fehler tut uns leid!</em>
    </li>
    <li>Fix - Fix missing filter that caused WooCommerce Product Bundles component items to be listed on the thank you page in conflict with the product page settings.
    </li>
    <li>Misc - Update WooCommerce tested version to 5.9.0
    </li>
  </ul>
  <p>
    <strong>Version 6.1.5 - 2021.11.8</strong>
  </p>
  <ul>
    <li>Improved - Added filter to control whether side cart items link to the product page. Filter: cfw_side_cart_link_item
    </li>
    <li>Fix - Fix bug where solid side cart icons fill color was set to none.
    </li>
    <li>Fix - Make sure elements with&nbsp;cfw-side-cart-open-trigger class have pointer cursor.
    </li>
  </ul>
  <p>
    <strong>Version 6.1.4 - 2021.11.5</strong>
  </p>
  <ul>
    <li>New - New side cart setting to hide floating side cart button when cart is empty.
    </li>
    <li>New - Order Bumps admin view now displays revenue that bump has captured. (Past revenue is estimated)
    </li>
    <li>Improved - When trust badge doesn't have a title or description, image is now displayed full width
    </li>
    <li>Improved - Added description to make it clear you can add embedded scripts to trust badge description for dynamic badges such as Norton Security.
    </li>
    <li>Improved - Added beta support for using Astra's header and footer on the checkout page. Requires loading theme styles which could cause conflicts.
    </li>
    <li>Improved - Set fill to none on side cart icon to prevent theme conflicts.
    </li>
    <li>Fix - Fix edge case where radio buttons had improper label styles.
    </li>
    <li>Fix - Fix bug where HTML tags ended up in field placeholders.
    </li>
    <li>If a label has an HTML tag present in it, display it as a conventional, non-floating label.&nbsp;
    </li>
    <li>Fix - Fix issue with UpSolution Core plugin by preventing it from loading styles on the checkout page.
    </li>
  </ul>
  <p>
    <strong>Version 6.1.3 - 2021.11.2</strong>
  </p>
  <ul>
    <li>Hotfix - Fix bug that caused side cart links to open in a new tab/window.
    </li>
  </ul>
  <p>
    <strong>Version 6.1.2 - 2021.11.2</strong>
  </p>
  <ul>
    <li>Improved - Side Cart item titles and images now link to the product page.
    </li>
    <li>Improved - When enabling cart item links in CheckoutWC &gt; Cart Summary, both title and image now link to the product page.
    </li>
    <li>Fix - Fix issue with WooCommerce Advanced Shipping that caused shipping to be rendered as 'Free!' inappropriately
    </li>
    <li>Fix - Fix JS error when no payment methods are available.
    </li>
    <li>Fix - When applying a coupon, any notices that appear will be cleared on the next AJAX refresh.
    </li>
    <li>Fix - Fix an issue with Avada that caused inline styles to be rendered to the page when they shouldn't be.
    </li>
    <li>Fix - Fix some German translations in de_DE and de_DE_formal
    </li>
    <li>Fix - Fix issue with Side Cart where inclusive taxes (VAT) was not handled properly when calculating the free shipping amount remaining.
    </li>
    <li>Fix - Fix issue where stat collector only sent 6 days of stats instead of 7.
    </li>
    <li>Fix - Fix issue where stat collector sent staging site stats.
    </li>
  </ul>
  <p>
    <strong>Version 6.1.1 - 2021.10.27</strong>
  </p>
  <ul>
    <li>Fix - Fix styling issue with secondary buttons such as the apply coupon button.
    </li>
  </ul>
  <p>
    <strong>Version 6.1.0 - 2021.10.27</strong>
  </p>
  <ul>
    <li>New - Added icon picker to Side Cart options!
    </li>
    <li>New - Added settings for side cart icon width and color.
    </li>
    <li>New - Added option to enable coupons on side cart.
    </li>
    <li>New - Added shortcode for placing a side cart launcher anywhere on your site. [checkoutwc_cart]
    </li>
    <li>Improved - Improved how order bumps are shown in side cart so they don't cover the cart items on small mobile devices.
    </li>
    <li>New - Added action to allow adding content when side cart is empty: checkoutwc_empty_side_cart_content
    </li>
    <li>Fix - Fix when no shipping method is selected, don't show 'Free!'
    </li>
    <li>Fix - Fix issue with Avada 7.5
    </li>
    <li>Fix - Fix issue where AJAX refresh happens twice on initial page load.
    </li>
    <li>Fix - Fix an issue with mobile
    </li>
    <li>Fix - Fix issue with SplitIt gateway
    </li>
    <li>Fix - Fix JS error with state not being a part of locale object.
    </li>
    <li>Fix - Fix left over var_dump in UpdatesManager.
    </li>
    <li>Fix - Fix subtle styling bug with accordions that has been lurking forever.
    </li>
  </ul>
  <p>
    <strong>Version 6.0.7 - 2021.10.22</strong>
  </p>
  <ul>
    <li>Improved - Added filters to WooCommerce Gift Cards output to allow heading, label, and placeholder to be changed.
    </li>
    <li>Fix - Disable JS that smoothly resized country, postcode, and state fields when switching countries because it's causing major the mobile view to zoom in and zoom out during refreshes on some sites.
    </li>
    <li>Fix - Account exists check was firing even when email field was empty.
    </li>
    <li>Fix - Fix issue where turning off checkout cart editing feature turned off the ability to change quantities or remove items on the side cart.
    </li>
  </ul>
  <p>
    <strong>Version 6.0.6 - 2021.10.21</strong>
  </p>
  <ul>
    <li>New - Added Romanian translations
    </li>
    <li>Improved - Order bumps now appear in the side cart when you enable the option in WP Admin &gt; CheckoutWC &gt; Side Cart
    </li>
    <li>Improved - Improved side cart styling
    </li>
    <li>Improved - Refactored Google Address Autocomplete JS&nbsp;
    </li>
    <li>Improved - Refactored Fetchify Address Autocomplete JS and
    </li>
    <li>Fix - Fix bug where Plus plan holders could see Side Cart settings in admin. Settings are now hidden unless you are a Pro or Agency license holder.
    </li>
    <li>Fix - Fixed styling issues with Fetchify Address Autocomplete and Glass theme / admin bar
    </li>
    <li>Fix - de_DE_formal is now a separate locale from de_DE. Thanks,&nbsp;JÃ¶rg!
    </li>
    <li>Fix - Free Shipping progress bar now shows decimal values when necessary.
    </li>
    <li>Fix - Fix more CSS conflicts with Side Cart and random themes and plugins
    </li>
  </ul>
  <p>
    <strong>Version 6.0.5 - 2021.10.16</strong>
  </p>
  <ul>
    <li>Improved - Implement woocommerce_cart_item_class so that plugins that need it can use it.
    </li>
    <li>Fix - Harden up styles to help mitigate Side Cart styling conflicts with themes.
    </li>
    <li>Fix - Fix issue where Resurs gateway needs classes on parent element to be in a specific order. (Yes, you read that right)
    </li>
    <li>Fix - Fix bug with merging locale data that resulted in JS errors for some stores.
    </li>
    <li>Fix - Prevent Astra Addon from loading styles on the checkout page.
    </li>
    <li>Fix - Fix date picker z-index with Local Pickup Plus.
    </li>
    <li>Fix - Fix bug with how we ran our AJAX updates on the checkout page that resulted in update_shipping_method not being set on requests. This caused major issues with Local Pickup Plus.
    </li>
    <li>Fix - Fix Fetchify styling.
    </li>
    <li>Fix - Fix responsive styles between mobile and desktop sizes where styling was broken.
    </li>
    <li>Fix - Implemented jQuery.scroll_to_notices from WooCommerce core for compatibility.&nbsp;<em>This should also fixes JS errors with WooCommerce PayPal Payments.</em>
    </li>
    <li>Fix - Make primary action button on mobile 100% width and place it before the secondary action (such as 'Return to shipping method')
    </li>
    <li>Fix - Fix issue where place order button was not 100% width on mobile.
    </li>
    <li>Fix - Fix styling of breadcrumbs on Futurist template.
    </li>
  </ul>
  <p>
    <strong>Version 6.0.4 - 2021.10.13</strong>
  </p>
  <ul>
    <li>Hotfix - Remove PHP 7.4 only code that causes fatal errors on older servers.
    </li>
  </ul>
  <p>
    <strong>Version 6.0.3 - 2021.10.12</strong>
  </p>
  <ul>
    <li>Improved - Forcefully re-enable cart fragment system when side cart is active.
    </li>
    <li>Fix - Fix bug where WooCommerce would redirect somewhere else instead of opening Side Cart. (When Side Cart is enabled our 'Skip cart step' feature is ignored)
    </li>
    <li>Fix - Fix bug where side cart didn't open on adding an item to cart if AJAX add to cart was turned off.
    </li>
    <li>Fix - Tweak styling of side cart to give header some more room to breathe.
    </li>
    <li>Fix - Native WooCommerce 'View cart' buttons should now open side cart.
    </li>
    <li>Fix - Added aria-label to floating cart button for screen readers.
    </li>
    <li>Fix - Fix potential fatal errors.
    </li>
    <li>Fix - Fix bug with SmartyStreets where it would break if your lookups were depleted.
    </li>
    <li>Fix - Fix bug with SmartyStreets where multiple requests were made for each lookup.
    </li>
    <li>Fix - Fix bug with SmartyStreets where modal would not close when clicking button to accept address.
    </li>
    <li>Fix - Fix esoteric bug with Resurs Bank gateway.
    </li>
    <li>Fix - Fix admin label for Side Cart 'Free Shipping Message'
    </li>
    <li>Fix - Use native WooCommerce unknown error message when gateway returns failure with no error messages.
    </li>
  </ul>
  <p>
    <strong>Version 6.0.2 - 2021.10.11</strong>
  </p>
  <ul>
    <li>Fix - Fix translation of continue shopping button
    </li>
    <li>Fix - Fix fatal error when cart or order item thumbnail is null
    </li>
    <li>Fix - Fix box-sizing issue that was causing things to render a few pixels offset
    </li>
    <li>Fix - Stop Flatsome from uppercasing cart item titles in side cart
    </li>
    <li>Fix - Stop Storefront theme from adding animation spinner to side cart update blockUI styling
    </li>
    <li>Fix - Fix issue with Futurist template breadcrumbs wrapping
    </li>
    <li>Fix - Fix issue where Futurist breadcrumb accents where missing
    </li>
  </ul>
  <p>
    <strong>Version 6.0.1 - 2021.10.08</strong>
  </p>
  <ul>
    <li>Improved - Add a separate setting for the background color of the free shipping progress bar.
    </li>
    <li>Fix - Fix issues with Side Cart and glass theme.
    </li>
  </ul>
  <p>
    <strong>Version 6.0.0 - 2021.10.08</strong>
  </p>
  <ul>
    <li>NEW! Side Cart is here and it's beautiful and lightning fast. Adding items to the cart opens a flyout cart from the right side of the screen that perfectly matches the cart experience on the checkout page and includes extras like a free shipping progress bar. This feature is available to all Pro plan and above subscribers. <a href="https://demo2.checkoutwc.com">You can see a demo here.</a>
    </li>
    <li>NEW! International Phone Field allows merchants to validate that the phone number entered is a valid phone number in the country selected. And it allows you to choose how the phone is stored when the order is submitted - this can help greatly with fulfillment services that require a specific format and valid phone numbers to work correctly.
    </li>
    <li>Improved - Upgraded Bootstrap grid from 4.x to 5.x
    </li>
    <li>Improved - Various performance improvements.
    </li>
    <li>Fix - Fixed issue on checkout page where quantity bubble on cart items was cut off.
    </li>
    <li>Fix - Lots of other little fixes we found. You know, the real 6.0 release is the commits we made along the way.
    </li>
  </ul>
  <p>
    <strong>Version 5.3.11 - 2021.10.04</strong>
  </p>
  <ul>
    <li>Hotfix - Ok, we didn't get that quite right:<br />
      <p>
        Fix cfw_get_shipping_total()
      </p>
      <p>
        Essentially invert logic of cfw_get_shipping_total() so that it follows the logic of WooCommerce's cart/cart-shipping.php template by first checking the available methods, and then descending into other checks.
      </p>
      <p>
        This also requires changing how cfw_show_shipping_total() determines whether to show the shipping total. Since error states are part of the shipping total, those are pushed further down to cfw_get_shipping_total() and instead we only check that we have shipping enabled and that the cart has items.
      </p>
    </li>
  </ul>
  <p>
    <strong>Version 5.3.10 - 2021.10.04</strong>
  </p>
  <ul>
    <li>Fix - Fix bug that caused 'Enter your address to view shipping options' to be displayed when the phone field was empty
    </li>
    <li>Improved - Refactor how we handle activation / deactivation routines
    </li>
  </ul>
  <p>
    <strong>Version 5.3.9 - 2021.09.27</strong>
  </p>
  <ul>
    <li>Improved - Add skip cart feature in CheckoutWC &gt; Checkout
    </li>
    <li>Fix - Fix bug that caused 'Free!' to show up on some orders where a shipping address had not been entered.
    </li>
    <li>Fix - Fix bug with SmartyStreets that caused the continue to payment button to be shown when it shouldn't be.
    </li>
    <li>Fix - Fix bug with Order Bumps when Offer Product is deleted.
    </li>
  </ul>
  <p>
    <strong>Version 5.3.8 - 2021.09.16</strong>
  </p>
  <ul>
    <li>Hotfix - Fix issue with styling of payment methods / billing address accordions on Glass theme
    </li>
  </ul>
  <p>
    <strong>Version 5.3.7 - 2021.09.15</strong>
  </p>
  <ul>
    <li>New - Bumped minimum PHP version to 7.1 since one of our existing dependencies already required PHP 7.1, setting an implicit minimum version.
    </li>
    <li>Fix - Fix bug with WooCommerce payments where the radio button for selecting credit card disappeared.
    </li>
    <li>Fix - Fix bug where shipping methods were blocked and wouldn't unblock
    </li>
    <li>Fix - Fix for Avada thank you page and view order page
    </li>
    <li>Fix - Fix for Avada styling of HTML element
    </li>
    <li>Fix - Fix for WooCommerce Gift Cards and coupon code AJAX. Now uses native WooCommerce AJAX for applying coupons.
    </li>
    <li>Fix - Fix a poorly translated French phrase.
    </li>
    <li>Fix - Fix up WooCommerce Shipment Tracking output and remove duplication
    </li>
    <li>Fix - Move theme styles / scripts suppression code outside of CompatbilityAbstract so it only runs once.
    </li>
    <li>Fix - Fix issue with whitespace on the right side of page on iPhones when using WooCommerce PayPal Payments
    </li>
    <li>Fix - Don't show optional in placeholder for fields that Brazillian Market changes
    </li>
    <li>Improved - Added filter for distraction free portal template redirect priority: cfw_template_redirect_priority
    </li>
    <li>Improved - Added filter for disabling existing account lookup by email: cfw_enable_account_exists_check
    </li>
    <li>Improved - Run initial AJAX update on page load faster (same speed as WooCommerce native checkout page)
    </li>
    <li>Improved - Added filter for determining when an order bump displays: cfw_display_bump
    </li>
  </ul>
  <p>
    <strong>Version 5.3.6 - 2021.09.03</strong>
  </p>
  <ul>
    <li>Improved - Tightened up timing of first AJAX refresh on checkout page to match core WooCommerce.
    </li>
    <li>Improved - Added support for Post NL 4.x
    </li>
    <li>Improved - If no valid shipping methods are available we now hide the 'Continue to payment' button to avoid confusion
    </li>
    <li>Fix - Fix issue with thank you page and Avada theme
    </li>
    <li>Fix - Protect against null cart items causing fatal error
    </li>
    <li>Fix - Fix order bumps fetch to include more than 5 items.
    </li>
    <li>Fix - Fix Klaviyo bug that caused the SMS notice to be separated from the checkbox.
    </li>
    <li>Fix - Fix Klaviyo bug where SMS checkbox had same name as newsletter checkbox.
    </li>
    <li>Fix - Fix potential styling issues with WooCommerce PayPal Payments when "Pay in X" notice is present
    </li>
    <li>Fix - Fix duplicated checkboxes with latest Klaviyo plugin update.<strong>&nbsp;(Please update Klaviyo after installing this release)</strong>
    </li>
    <li>Tweak - Slightly changed output position of Klaviyo checkboxes.
    </li>
    <li>Tweak - Added $mobile boolean variable to cfw_before_coupon_module action
    </li>
  </ul>
  <p>
    <strong>Version 5.3.5 - 2021.08.20</strong>
  </p>
  <ul>
    <li>Improved - Support WooCommerce 5.6.0 built in support for Shipping Phone field.
    </li>
    <li>Improved - Add compatibility for WooCommerce Gift Cards coupon input add-on plugin
    </li>
    <li>Improved - Switch Amazon Pay logo to SVG for vector retina rendering goodness.
    </li>
  </ul>
  <p>
    <strong>Version 5.3.4 - 2021.08.04</strong>
  </p>
  <ul>
    <li>Fix - Fix express checkout button rendering for WooCommerce payments.
    </li>
  </ul>
  <p>
    <strong>Version 5.3.3 - 2021.08.04</strong>
  </p>
  <ul>
    <li>Improved - Beta Support for WooCommerce Payments express checkout buttons. This is largely untested due to the difficult of testing WooCommerce Payments in a dev environment. Please let us know if it works for you.
    </li>
    <li>Improved - Added additional CSS custom properties that make it possible to control loading "shimmer" animation during refreshes
    </li>
    <li>Fix - Fix location of mobile coupon output. Now appears above the payment methods as described by the option in CheckoutWC &gt; Checkout
    </li>
    <li>Fix - Fix a potential fatal error
    </li>
    <li>Fix - Order Bumps filter no longer appears on the orders list when there are no order bumps
    </li>
    <li>Fix - Shore up order submission JS to match WooCommerce core more closely
    </li>
    <li>Fix - Make sure wc_checkout_params.checkout_url is the right AJAX submission endpoint on our checkout page
    </li>
    <li>Fix - Fix issue with YITH points and Rewards notice not appearing
    </li>
  </ul>
  <p>
    <strong>Version 5.3.2 - 2021.07.21</strong>
  </p>
  <ul>
    <li>New - Futurist theme now has full access to breadcrumb color settings
    </li>
    <li>Improved - Added cfw_klaviyo_output_hook filter to determine where Klaviyo outputs its stuff
    </li>
    <li>Improved - Added cfw_shipping_free_text filter to set the text when shipping is free
    </li>
    <li>Fix - Fix issue with location of cfw_before_payment_method_heading action and fragment updates
    </li>
    <li>Fix - Update German translation of promo code
    </li>
    <li>Fix - Fix issue with mismatched label and placeholder for fields like post code based on country locale strings from WooCommerce core
    </li>
  </ul>
  <p>
    <strong>Version 5.3.1 - 2021.07.10</strong>
  </p>
  <ul>
    <li>Fix - Fix issue where company field didn't trigger a refresh.
    </li>
    <li>Fix - Fix cart summary mobile background color with new settings scheme. Added a new Cart Summary Mobile Background Color setting
    </li>
    <li>Fix - Fix issue where current order status was not reflected when viewing an order if the current status was not set as one of the status progressions in the Thank You Page settings.
    </li>
  </ul>
  <p>
    <strong>Version 5.3.0 - 2021.07.6</strong>
  </p>
  <p>
    This is a pretty big release!&nbsp; <strong>As always, we recommend testing on a staging site before updating your live site!</strong>
  </p>
  <ul>
    <li>New - Added new address autocomplete service - <a href="https://www.checkoutwc.com/documentation/fetchify-address-autocomplete">Fetchify</a>!
    </li>
    <li>New - Filter WooCommerce Admin orders screen by whether the order contains Order Bumps.
    </li>
    <li>New - New color settings for breadcrumbs and accent colors.
    </li>
    <li>New - Refactored color settings to use Custom CSS Properties.
    </li>
    <li>New - It's now possible to remove cart items that don't have an adjustable quantity.
    </li>
    <li>New - Added option to CheckoutWC &gt; General to hide the CheckoutWC admin menu bar button on non-CheckoutWC pages.
    </li>
    <li>Improved - Added cfw_is_thank_you_page_active() function to let developers determine if the thank you page is turned on.
    </li>
    <li>Improved - Fields with attribute data-persist=false won't be locally cached with Garlic.
    </li>
    <li>Improved - JS build target moved from es5 to es2015.
    </li>
    <li>Improved - Changing company field now refreshes checkout since it is visible in the order review panes.
    </li>
    <li>Fix - Fix issue with account exists checks running even when login form was set to use WooCommerce login.
    </li>
    <li>Fix - Fix issue with WooCommerce PayPal Payments fields rendering with the wrong size.
    </li>
    <li>Fix - Fix visual glitch with rounded borders on accordions (shipping methods, payment methods, billing address) that caused the border to have a small white break at the corners
    </li>
    <li>Fix - Fix issues with SmartyStreets and address_2
    </li>
    <li>Fix - Fix issue with Klaviyo checkbox being output twice.
    </li>
    <li>Fix - Fix issue with order bump not showing if offer product stock wasn't managed.
    </li>
    <li>Fix - Fix issue with Php Snippets and the backslash character.
    </li>
    <li>Fix - Fix PHP warning with WooCommerce Square gateway
    </li>
    <li>Fix - Fix refactored how we handle shipping totals to more accurately display conditions such as no shipping methods being available, especially when using more than one shipping package.
    </li>
    <li>Fix - If value exists on page load, don't override it with Garlic.
    </li>
    <li>Fix - Removed cfw-field-persistence-loaded JS event since it didn't work.
    </li>
    <li>Fix - Fix issue with CartFlows React UI.
    </li>
    <li>Fix - Fix issue where billing_email didn't match logged in user's email.
    </li>
    <li>Fix - Fix mobile styling issue with WooCommerce notices that contain buttons.
    </li>
    <li>Fix - Fix issue with Parsley field validation message translation and Weglot.
    </li>
  </ul>
  <p>
    <strong>Version 5.2.4 - 2021.07.02</strong>
  </p>
  <ul>
    <li>Hotfix - Fix issue with Avada 7.3.1
    </li>
  </ul>
  <p>
    <strong>Version 5.2.3 - 2021.06.15</strong>
  </p>
  <ul>
    <li>Fix - Fix issue with WooCommerce Germanized checkboxes next to the place order button
    </li>
  </ul>
  <p>
    <strong>Version 5.2.2 - 2021.06.14</strong>
  </p>
  <ul>
    <li>Hotfix - Fixes for Avada 7.4. <a href="https://www.checkoutwc.com/documentation/avada-template-layout-problems">PLEASE READ THIS DOC BEFORE CONTACTING SUPPORT.</a>
    </li>
  </ul>
  <p>
    <strong>Version 5.2.1 - 2021.06.14</strong>
  </p>
  <ul>
    <li>Hotfix - Fix output of WooCommerce Germanized checkboxes
    </li>
  </ul>
  <p>
    <strong>Version 5.2.0 - 2021.06.10</strong>
  </p>
  <ul>
    <li>New - Order Bumps can now be configured to show if one or more category of products is in the cart!
    </li>
    <li>New - Support for ConverKit for WooCommerce
    </li>
    <li>Improved - If an Order Bump becomes invalid because the cart changed, we "undiscount" the bump until the cart satisfies the bump conditions.
    </li>
    <li>Improved - Added JavaScript validation to Order Bumps editor.
    </li>
    <li>Improved - When showing discounts on cart items, render Order Bumps price correctly.
    </li>
    <li>Fix - Fix issue with WooCommerce PayPal Payments that caused the PayPal buttons not to appear.
    </li>
    <li>Fix - You can no longer select a variable product parent as an offer product.
    </li>
    <li>Fix - Bumps cannot satisfy the display conditions for other bumps.
    </li>
    <li>Fix - Fix compatibility with woocommerce_checkout_redirect_empty_cart and woocommerce_checkout_update_order_review_expired hooks.
    </li>
    <li>Fix - Added a workaround for Authorize.net and order review step
    </li>
  </ul>
  <p>
    <strong>Version 5.1.2 - 2021.06.09</strong>
  </p>
  <ul>
    <li>Hotfix - Fix issue with Chrome autofilling fields bug and one page checkout setting.
    </li>
  </ul>
  <p>
    <strong>Version 5.1.1 - 2021.06.08</strong>
  </p>
  <ul>
    <li>Fix - Fixes for Klaviyo SMS checkbox and disclaimer location
    </li>
    <li>Fix - Fix issue with Trusted Payments gateway
    </li>
    <li>Fix - Fix issue where express checkout container showed up when no express buttons were present
    </li>
    <li>Fix - Fix bug with Chrome autofilling fields on previous steps
    </li>
    <li>Fix - Fix admin conflict with Formidable Forms and MapSVG
    </li>
  </ul>
  <p>
    <strong>Version 5.1.0 - 2021.06.04</strong>
  </p>
  <ul>
    <li>New! Order Bumps can now be used as Upsells. Check out our documentation here: <a href="https://www.checkoutwc.com/documentation/order-bumps">https://www.checkoutwc.com/documentation/order-bumps/</a>
    </li>
    <li>New - Support for WooCommerce Pakettikauppa
    </li>
    <li>New - Support for Woo Finvoicer
    </li>
    <li>Fix - Fix issues with TM Extra Product Options and Order Bump discounts
    </li>
    <li>Fix - Add login prompt to PayPal for WooCommerce review order screen
    </li>
    <li>Fix - Fix issue with WooCommerce Checkout Fields Editor Pro from Acoweb where fields were readonly
    </li>
    <li>Fix - Add beta support for ThemeHigh's popular Checkout Field Editor.&nbsp;
    </li>
    <li>Fix - Fix issues with WooCommerce Juno
    </li>
    <li>Fix - Fix issues with Brazilian Market on WooCommerce
    </li>
    <li>Fix - Fix JavaScript error in express checkout button check
    </li>
    <li>Fix - Fix validation of extra shipping fields where fields don't have labels
    </li>
    <li>Fix - Fix styling of select2/selectWoo select fields
    </li>
  </ul>
  <p>
    <strong>Version 5.0.5 - 2021.05.27</strong>
  </p>
  <ul>
    <li>Fix - Fix issue with Parsley validation of checkboxes
    </li>
    <li>Fix - Fix translation for WooCommerce Gift Cards
    </li>
    <li>Fix - Fix issue where Elementor header / footer didn't show up on thank you page
    </li>
    <li>Fix - WP admin bar now shows up on thank you page if you're logged in
    </li>
    <li>Fix - Fix issue with Spanish addresses autocompleting state incorrectly
    </li>
    <li>Fix - Fix issue with fields laying out incorrectly when country switched
    </li>
    <li>Fix - Fix button styling on address verification modal (SmartyStreets)
    </li>
    <li>Fix - Billing address is always shown when Brazilian Market on WooCommerce is active.
    </li>
    <li>Fix - Fix glitches with payment request buttons container showing up when no buttons were available.
    </li>
  </ul>
  <p>
    <strong>Version 5.0.4 - 2021.05.20</strong>
  </p>
  <ul>
    <li>Fix - Fix problem with PayPal for WooCommerce that caused billing address fields to not sync over correctly from logged in session.
    </li>
    <li>Fix - Fix PHP warning
    </li>
    <li>Fix - Fix issue where Trust Badge didn't appear to save unless you added an image
    </li>
    <li>Fix - Fix how trust badges lay out on frontend without images
    </li>
    <li>Fix - Adjusted priorities of address fields to match core more closely
    </li>
  </ul>
  <p>
    <strong>Version 5.0.3 - 2021.05.19</strong>
  </p>
  <ul>
    <li>Fix - Fix bug with one page checkout not firing order submit handlers properly.
    </li>
    <li>Fix - Fix styling bugs with content loader.
    </li>
    <li>Fix - Fix JS errors with Amazon Pay.
    </li>
    <li>Fix - Fix bug with create account checkbox not auto checking.
    </li>
    <li>Fix - Fix PHP 8 deprecation notice.
    </li>
  </ul>
  <p>
    <strong>Version 5.0.2 - 2021.05.18</strong>
  </p>
  <ul>
    <li>Hotfix: Fix issue where billing address fields weren't synced from shipping address fields.
    </li>
    <li>Fix: Fix glitches with admin bar
    </li>
    <li>Fix: Fix issue with view order URL being styled incorrectly
    </li>
    <li>Fix: Fix issue with styling of checkboxes
    </li>
    <li>Fix: Fix issue with Canada city being filled improperly with Google Address Autocomplete.
    </li>
    <li>Fix: Fix issue where Amazon button could render incorrectly for a few seconds.
    </li>
    <li>Improved: Added mechanism for custom validation of custom fields with parsley.js
    </li>
  </ul>
  <p>
    <strong>Version 5.0.1 - 2021.05.18</strong>
  </p>
  <ul>
    <li>Hotfix: Fix bug where translations did not load
    </li>
    <li>Hotfix: Fix bug where Trust Badges settings did not appear to save
    </li>
  </ul>
  <p>
    <strong>Version 5.0.0 - 2021.05.17</strong>
  </p>
  <p>
    Major new version! This release comprises over 700 commits - we didn't hold back. We're excited for you to try it, but you should do proper testing before updating.&nbsp; <strong>Before updating your live site, PLEASE TEST ON STAGING.</strong>
  </p>
  <ul>
    <li>New - Order Bumps (Pro or higher plan)
    </li>
    <li>New - SmartyStreets Address Validation (Pro or higher plan)
    </li>
    <li>New - Trust Badges
    </li>
    <li>New - Footer menu location for adding footer links to the checkout page.
    </li>
    <li>New - Redesigned admin pages
    </li>
    <li>New - Estonian translations
    </li>
    <li>Improved - Support for latest Square gateway express buttons (Apple Pay, Google Pay, etc)
    </li>
    <li>Improved - Refactored code base for faster more robust performance
    </li>
    <li>Fix - Fix issue with Alabama being selected by default when it shouldn't be
    </li>
  </ul>
  <p>
    <strong>Version 4.3.8 - 2021.05.11</strong>
  </p>
  <ul>
    <li>Hotfix: Fix Amazon Pay. Should work with Amazon Pay 1.0 and Amazon Pay 2.0, including both the legacy integration method and the new API. However, the new API is&nbsp;<strong>NOT fully tested</strong>&nbsp;due to the urgent nature of releasing this fix.&nbsp;<strong>We do NOT recommend you reconnect to the Amazon API until you have&nbsp;<em>FULLY</em>&nbsp;tested on a staging site.</strong>
    </li>
    <li>Fix - Fix glitch with non-shipped orders and PayPal for WooCommerce review screen.
    </li>
    <li>Fix - Fix some styling issues with CommerceKit
    </li>
    <li>Improved - Added cfw_thank_you_page_map_address filter to allow overriding the map address on the thank you page.
    </li>
    <li>Improved - Added symlink for de_DE_formal locale to de_DE.
    </li>
  </ul>
  <p>
    <strong>Version 4.3.7 - 2021.05.06</strong>
  </p>
  <ul>
    <li>Fix - Fix how we set language for Google Address Autocomplete
    </li>
    <li>Fix - Fix fatal error with old version of Klaviyo by adding version check
    </li>
  </ul>
  <p>
    <strong>Version 4.3.6 - 2021.05.04</strong>
  </p>
  <ul>
    <li>Improved - Set language for Google Places library so that autocomplete suggestions are in the correct locale
    </li>
    <li>Fix - Fix Klaviyo newsletter checkbox position
    </li>
    <li>Fix - Fix issue with WooCommerce Conditional Shipping and Payments notices not being displayed on update_checkout
    </li>
  </ul>
  <p>
    <strong>Version 4.3.5 - 2021.04.26</strong>
  </p>
  <ul>
    <li>Hotfix - Fix invalid reference to settings manager in WooCommerce Germanized compatibility class.
    </li>
  </ul>
  <p>
    <strong>Version 4.3.4 - 2021.04.26</strong>
  </p>
  <ul>
    <li>New - Compatibility with Neve theme
    </li>
    <li>New - Vietnamese translations
    </li>
    <li>Fix &nbsp;- Fix bugs with validation of billing address when order review step is enabled
    </li>
    <li>Fix - Fix styling issues with order review step total
    </li>
    <li>Fix - Parse house number if Google Maps doesn't have address in their DB
    </li>
    <li>Fix - Workaround for Dutch addresses and Address Autocomplete to properly map city field
    </li>
    <li>Fix - Fix for WooCommerce Germanized terms and conditions and order review step
    </li>
  </ul>
  <p>
    <strong>Version 4.3.3 - 2021.04.01</strong>
  </p>
  <ul>
    <li>Fix - Fix PHP 8 warnings / notices.
    </li>
    <li>Fix - Fix for Uncode theme
    </li>
    <li>Fix - Fixes for Avada 7.3
    </li>
    <li>Fix - Fix for Stripe (official) gateway that prevented Apple Pay / Google Pay when phone fields were required.
    </li>
  </ul>
  <p>
    <strong>Version 4.3.2 - 2021.03.30</strong>
  </p>
  <ul>
    <li>Fix - Fix bug with WooCommerce Germanized where cart items were not visible
    </li>
    <li>Fix - Fix issue with Stripe for WooCommerce and iDEAL that made the bank dropdown not selectable.
    </li>
    <li>Fix - Fix PHP 8 warnings.
    </li>
  </ul>
  <p>
    <strong>Version 4.3.1 - 2021.03.29</strong>
  </p>
  <ul>
    <li>Hotfix - Fix issue where gateway icons could be way too tall.
    </li>
    <li>Hotfix&nbsp;- Fix issue where AJAX requests response was being cached occasionally in Safari.
    </li>
  </ul>
  <p>
    <strong>Version 4.3.0 - 2021.03.26</strong>
  </p>
  <ul>
    <li>ðŸŽ¨ New: During refreshes checkout sections now have a sweet new 'loading shimmer' effect rather than fading out.&nbsp;
    </li>
    <li>Improved: Page now refreshes faster on first load
    </li>
    <li>Improved: Added missing aria description to field output.
    </li>
    <li>Fix - Fix edge cases where fatal error could be fired if a shipping method isn't a proper shipping method.
    </li>
    <li>Fix - Fix bug that caused fractional quantities like 0.5 to remove an item from the cart.
    </li>
    <li>Fix - Fix issue where billing address fields were synced from shipping address at the wrong time on page load. Now happens after field values have been restored from cache.
    </li>
    <li>Fix - Fix styling of cart total on mobile
    </li>
    <li>Fix - Fix issue where JS error was thrown when Checkout Add-ons for WooCommerce was activated.
    </li>
    <li>Fix - Fix bug where post code was not set to optional or required properly when switching countries.
    </li>
    <li>Fix - Fix bugs with Stripe and Order Review Step feature.
    </li>
    <li>Fix - Fix issue with New Zealand addresses and Google Address Autocomplete.
    </li>
    <li>Fix - Fix improper implementations of debounced that were not debouncing.
    </li>
    <li>Fix - Fix issue where cart items were being modified during refresh when there were no changes.
    </li>
    <li>Fix - Fix bug with custom attributes on fields that caused them to be output improperly.
    </li>
    <li>Fix - Fix bug with Free Gifts for WooCommerce that caused items not to show up when cart was modified to satisfy gift conditions.
    </li>
  </ul>
  <p>
    <strong>Version 4.2.0 - 2021.03.18</strong>
  </p>
  <ul>
    <li>Improved - Cart updates now happen in normal update_checkout refresh - saves an extra AJAX call.
    </li>
    <li>Improved - Performance: On page load, multiple AJAX refreshes would run. Now only one will run.&nbsp;
    </li>
    <li>Improved - All compatibility classes are now singletons with accessible instances&nbsp;
    </li>
    <li>Improved - Refactored compatibility module system to improve&nbsp;
    </li>
    <li>Improved - Some light refactoring of our JS to decouple the code and prepare for larger refactors later.
    </li>
    <li>Fix - Fix styling issue with coupons on Futurist theme.
    </li>
    <li>Fix - Fix bug where removing YITH composite product didn't remove components.
    </li>
    <li>Fix - Fix for Avada and the thank you page.
    </li>
    <li>Fix - Fix CSS conflict with Flatsome theme.
    </li>
    <li>Fix - Fix styling bugs with Klarna Checkout.
    </li>
    <li>Fix - Fix bugs with Brazilian Market
    </li>
    <li>Fix - Fix bug where Smart Coupons 'bounced' multiple times on page load
    </li>
    <li>Fix - Fix change how we resolve state with Google Address Autocomplete to handle more countries correctly
    </li>
  </ul>
  <p>
    <strong>Version 4.1.1&nbsp;- 2021.03.05</strong>
  </p>
  <ul>
    <li>New - Bulgarian translations
    </li>
    <li>Fix - &nbsp;Fix potential error in Avada compatibility module
    </li>
    <li>Fix - Fix bug with Address Autocomplete that resulted in house_number showing up in address field 1
    </li>
    <li>Fix - Fixes for Brazilian Market (Extra Checkout Fields for Brazil)
    </li>
    <li>Fix - Fixes for country / state field changes that resulted in inconsistent states or wrong labels.
    </li>
    <li>Fix - Fix JS error on order pay page that could prevent the page from functioning.
    </li>
  </ul>
  <p>
    <strong>Version 4.1.0 - 2021.02.26</strong>
  </p>
  <ul>
    <li>New - Added support for Sumo Subscriptions
    </li>
    <li>New - Added Czech translations
    </li>
    <li>Improved - Added custom event (cfw-fire-udpate-cart-action) for triggering update_cart event
    </li>
    <li>Improved - Added woocommerce_view_order hook (but surpassed default actions on hook that are redundant)
    </li>
    <li>Fix - Fix styling issue with Pro theme
    </li>
    <li>Fix - Fix issue with billing address sync from shipping fields to correct issues with gateways and ensure the session address data is properly stored / retrieved
    </li>
    <li>Fix - Fix issue with SEPA gateway and Stripe For WooCommerce (Payment Plugins)&nbsp;
    </li>
    <li>Fix - Fix for issue where other plugins look for a particular class when checking notices on page
    </li>
    <li>Fix - Fix issue with SplitIt payment gateway
    </li>
    <li>Fix - Prevent fatal errors when gateway isn't a proper gateway instance or no gateways are enabled
    </li>
  </ul>
  <p>
    <strong>Version 4.0.7 - 2021.02.22</strong>
  </p>
  <ul>
    <li>Hotfix: Fix another Amazon Pay issue that caused the shipping state to be hidden.
    </li>
    <li>Fix: Fix issue with Google Address autocomplete and premise / subpremises.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 4.0.6 - 2021.02.19</strong>
  </p>
  <ul>
    <li>Hotfix: Fix issue with latest Amazon Pay gateway update that caused the shipping address fields to be hidden.
    </li>
  </ul>
  <p>
    <strong>Version 4.0.5 - 2021.02.11</strong>
  </p>
  <ul>
    <li>Fix - Fix issues with SendCloud update.
    </li>
    <li>Fix - Fix issue with Flatsome and WooCommerce Germanized.
    </li>
    <li>Fix - Fix potential fatal error on thank you page.
    </li>
    <li>Fix - Fix styling for Google Pay button with Stripe for WooCommerce (PaymentPlugins) gateway.
    </li>
  </ul>
  <p>
    <strong>Version 4.0.4 - 2021.02.04</strong>
  </p>
  <ul>
    <li>New - Support for saved Addresses for WooCommerce.
    </li>
    <li>Fix - Fix bug with Woocommerce Side Cart Premium that caused endless refreshes when paired with Google Address Autocomplete feature.
    </li>
    <li>Fix - Fix inefficiency with Address Autocomplete feature that caused redundant events to be queued when using autocomplete more than once.
    </li>
    <li>Fix - Fix bug with TranslatePress that caused AJAX output to contain get text wrapping strings.
    </li>
    <li>Fix - Removed old Braintree for WooCommerce (PaymentPlugins) JS compatibility code that is no longer needed.
    </li>
  </ul>
  <p>
    <strong>Version 4.0.3 - 2021.02.01</strong>
  </p>
  <ul>
    <li>New - Added Korean (ko_KR) translations
    </li>
    <li>Fix - Fix issue where company wasn't sent with update_checkout
    </li>
    <li>Fix - Fix issue where shipping address review had stale data.
    </li>
    <li>Fix - Fix JS error when no payment methods are available.
    </li>
    <li>Fix - Fix issue where place order button HTML was not updated during refreshes.
    </li>
    <li>Fix - Fix issue with missing compatibility module JS&nbsp;
    </li>
    <li>Fix - Fix styling of Stripe for WooCommerce payment request buttons.
    </li>
    <li>Fix - Fix issue with payment gateway being reset to first selected gateway during refreshes.
    </li>
    <li>Fix - Fix issue where summary showed innert 'Change' links on PayPal for WooCommerce review page.
    </li>
  </ul>
  <p>
    <strong>Version 4.0.2 - 2021.01.22</strong>
  </p>
  <ul>
    <li>New - Added Croatian and Chinese Traditional (Taiwan) translations
    </li>
    <li>Enhanced - Removed vestigial cfw_updated_checkout event as some gateways had implemented it to correct issues that are no longer issues. This prevents potential problems from events running twice.
    </li>
    <li>Enhanced - Implemented woocommerce_quantity_input_max filter to make sure our quantity stepper obeys the rules on maximum quantity.
    </li>
    <li>Fix - Fix a few PHP notices.
    </li>
    <li>Fix - Fix issue where 'Change' link showed up by the shipping method in the review panels when 'Ship shipping step' was enabled.
    </li>
    <li>Fix - Fix issue where you could enter more than the allowed product quantity in the JS prompt that appears when you click 'Edit'.&nbsp;
    </li>
    <li>Fix - Fix issue where order review step totals didn't properly update.
    </li>
    <li>Fix - Fix issues when applying a coupon code that makes an order free.
    </li>
    <li>Fix - Fix issue where removing a 100% off (free) coupon resulted in the payment method label not being displayed in the review panels.
    </li>
  </ul>
  <p>
    <strong>Version 4.0.1 - 2021.01.15</strong>
  </p>
  <ul>
    <li>Hotfix: Fix bug with pre_option_ filter that caused WooCommerce style registration to fail.
    </li>
    <li>Update Norwegian translations.
    </li>
  </ul>
  <p>
    <strong>Version 4.0.0 - 2021.01.14</strong>
  </p>
  <p>
    This release took about 6 weeks to finish and over 117 commits. This release is more about refinements and thoughtful refactors than new features, but it does have some new features too!
  </p>
  <p>
    <strong>Please test carefully on a staging site before updating.</strong>There shouldn't be any breaking changes, but any release of this size is certain to have bugs that were missed during the development and testing processes.
  </p>
  <ul>
    <li>
      <strong>New Premium Feature:</strong>Order Review Step - Order Review Step adds a tab after the payment tab with a full summary of the order information and totals above the place order button. This should be especially helpful to German stores, and other stores located in jurisdictions that require full disclosure before order submission.
    </li>
    <li>
      <strong>Enhanced Remove Coupon:</strong>Removing coupons now happens with an AJAX refresh instead of reloading the page.
    </li>
    <li>
      <strong>New:</strong>Support for MyShipper&nbsp;
    </li>
    <li>
      <strong>New:</strong>Support for Iconic WooCommerce Delivery Slots
    </li>
    <li>
      <strong>New:</strong>Complete parity with WooCommerce core on checkout refreshes. We now fire updated_checkout on every refresh instead of selectively. Should iron out various glitches we have had with 3rd party add-ons.
    </li>
    <li>
      <strong>New:</strong>Lithuanian translations.&nbsp;
    </li>
    <li>
      <strong>New:</strong>Support for Shoptimizer
    </li>
    <li>
      <strong>Enhanced:</strong>It's now possible to use a filter and set a step amount for quantity adjustments.
    </li>
    <li>
      <strong>Enhanced:</strong>You can now click on the entire row of payment methods and other accordions rather than clicking specifically on the text label.&nbsp;
    </li>
    <li>
      <strong>Enhanced:</strong>Added various new filters. Documentation coming soon!
    </li>
    <li>
      <strong>Enhanced:</strong>Added docblock documentation for all our actions and filters to make updating our documentation easier.
    </li>
    <li>
      <strong>Enhanced:</strong>Refactored our compatibility class loader.
    </li>
    <li>Fix: Fixes for Local Pickup Plus
    </li>
    <li>Fix: Fixes for WooCommerce German Market
    </li>
    <li>Fix: Fixes for OceanWP themes
    </li>
    <li>Fix: Fixes for latest version of Avada theme
    </li>
    <li>Fix: Updates to French translations
    </li>
    <li>Fix: More robust parsing of error messages during checkout submit.
    </li>
    <li>Fix: Fix bugs with WooCommerce Country Based Payments
    </li>
    <li>Fix: Fix issues with WooCommerce Order Delivery Date
    </li>
    <li>Fix: Fix stale selector issue with payment method state cache during updates.
    </li>
    <li>Fix: Fix for Culqi payment gateway and other gateways that use the order pay receipt hook.
    </li>
    <li>Fix: Fix for error messages that could not be properly hashed.
    </li>
    <li>Fix: Fix for MyParcel styling
    </li>
    <li>Fix: Fix review pane address references to pickup changes and not pull from stale session info.
    </li>
    <li>Fix: Fix JS errors on order pay page.
    </li>
  </ul>
  <p>
    <strong>Version 3.13.3 - 2020.11.26</strong>
  </p>
  <ul>
    <li>New: Support for WooCommerce Subscription Gifting.
    </li>
    <li>Fix: Fix 'No shipping options' string to match WooCommerce core. This enables proper translation.
    </li>
  </ul>
  <p>
    <strong>Version 3.13.2 - 2020.11.23</strong>
  </p>
  <ul>
    <li>Fix: Revert Amazon Pay changes from 3.13.0 that caused issues with missing email fields.
    </li>
    <li>Add cfw_payment_methods_ul_start and cfw_payment_methods_ul_end actions.
    </li>
  </ul>
  <p>
    <strong>Version 3.13.1&nbsp;- 2020.11.19</strong>
  </p>
  <ul>
    <li>Hotfix: Fix tiny CSS styling issue with return to previous step links that caused them to break onto two lines.
    </li>
  </ul>
  <p>
    <strong>Version 3.13.0 - 2020.11.19</strong>
  </p>
  <ul>
    <li>New: CheckoutWC now works with <a href="https://woocommerce.com/products/recaptcha-for-woocommerce/" target="_blank">reCaptcha for WooCommerce</a>.
    </li>
    <li>New: Added support for WooCommerce Enhanced Coupon Features Pro.
    </li>
    <li>Improved: Refactored update_checkout AJAX refresh code to align it with WooCommerce core. This fixed some edge case bugs and simplified the code.
    </li>
    <li>Improved: We no longer hide settings from WooCommerce &gt; Settings &gt; Accounts &amp; Privacy. We mark them with an asterisk and a note so you know which ones may be overridden by CheckoutWC.
    </li>
    <li>Improved: Added an internal logging service for logging JS errors and events.
    </li>
    <li>Improved: Added some button styling for buttons in alerts.
    </li>
    <li>Fix: Don't show WPWeb Social Login buttons for logged in users.
    </li>
    <li>Fix: Fix issues with Pimwick Gift Cards. We're no longer doing a full integration with this plugin as the code is too brittle and requires us to copy their templates and then maintain them. Consequently, the gift card field will no longer show up under the promo card field.
    </li>
    <li>Fix: Fix issues with WordPress theme loader (still experimental) and Square gateway
    </li>
    <li>Fix: Fix issues with Checkout Add-ons and Select2 fields.
    </li>
    <li>Fix: Fix bug where admin area of Checkout Field Editor didn't hide unusable areas.
    </li>
    <li>Fix: Fix issue with WooCommerce Product Add-ons cart item data.
    </li>
    <li>Fix: Fix styling of Braintree / Stripe for WooCommerce payment request buttons (PaymentPlugins gateways)
    </li>
    <li>Fix: Fixed an undefined index notice.
    </li>
    <li>Fix: Fix mobile styling of mobile cart summary header.
    </li>
    <li>Fix: Fix cfw-payment-tab-loaded event
    </li>
    <li>Fix: Fix issue where Stripe CC field was rendered with an invisible placeholder on mobile safari / iOS.
    </li>
    <li>Fix: Fix issue where Amazon Pay button could show up and be unclickable.
    </li>
    <li>Fix: Added a way to re-enable field validation when using Amazon Pay. Filter: cfw_amazon_suppress_shipping_field_validation
    </li>
    <li>Fix: Fix WooCommerce translation that was misaligned with core causing the string to not be translated.
    </li>
    <li>Fix: Fix issue where a customer who downgraded their CheckoutWC license might be stuck with premium functionality turned on without anyway to turn it off.
    </li>
    <li>Fix: Fix styling issues with PayPal for WooCommerce order review screen on mobile.
    </li>
    <li>Fix: Fix issue where digital only orders could not be completed with PayPal for WooCommerce.
    </li>
    <li>Fix: Fix styling bug on review summary when order is not shipped.
    </li>
    <li>Fix: Added 'update' event from WooCommerce core to trigger update_checkout refresh.
    </li>
    <li>Fix: Fix bug with one-time shipping and WooCommerce Subscriptions.
    </li>
  </ul>
  <p>
    <strong>Version 3.12.2 - 2020.10.26</strong>
  </p>
  <ul>
    <li>Hotfix: Fix PHP error in Admin controller from typo in function name.
    </li>
  </ul>
  <p>
    <strong>Version 3.12.1 - 2020.10.23</strong>
  </p>
  <ul>
    <li>Hotfix: Fix fatal error with WooCommerce Thank You Page - NextMove Plugin. Adds missing parameter to body_class filter.
    </li>
  </ul>
  <p>
    <strong>Version 3.12.0 - 2020.10.22</strong>
  </p>
  <p>
    Note: This release eliminates translation of strings in the CheckoutWC admin settings screens.&nbsp;
  </p>
  <ul>
    <li>New: Click to see promo code option. Adds a link 'Have a promo code? Click here.'
    </li>
    <li>New: Tooltip on CVV fields with explanatory text for users.
    </li>
    <li>New: New 'Edit' link on cart items that appears on hover. Allows users to make larger edits to quantity of an item.
    </li>
    <li>Improved: Mobile cart summary now has a cart icon and a 'Hide order summary' link when opened.&nbsp;
    </li>
    <li>Improved: Added Billing Address subheading.
    </li>
    <li>Improved: Shortened Payments subheading text.
    </li>
    <li>Improved: Added class to cart items that are components of YITH Composite products for easier styling.
    </li>
    <li>Fix: Fixed issue with Elementor global styles not working on checkout page.
    </li>
    <li>Fix: Fixed styling issues with BACS gateway on thank you page.
    </li>
    <li>Fix: Fixed bug with Glass theme and Stripe for WooCommerce that caused Google Pay / Apple Pay to always be styled as selected.
    </li>
    <li>Fix: Added support for Extra Fees for WooCommerce.
    </li>
    <li>Fix: Fixed translation bug with English (UK) translations.
    </li>
    <li>Fix: Fixed bug with Checkout Add-ons select input labels not appearing.
    </li>
    <li>Fix: Fixed bug with SendCloud JS compatibility code.
    </li>
    <li>Fix: Added back AJAX output error suppression.
    </li>
    <li>Fix: Added protection to avoid fatal errors during WooCommerce upgrades.
    </li>
    <li>Fix: Fix styling for really long email addresses.
    </li>
    <li>Other: Removed translations for admin screens. This will speed up future development by eliminating 75% of the strings we have to manage with releases.
    </li>
    <li>Other: Updated tested versions to WooCommerce 4.6.1.
    </li>
  </ul>
  <p>
    <strong>Version 3.11.1 - 2020.10.10</strong>
  </p>
  <ul>
    <li>Hotfix: Fix issue where submitting checkout with PayPal for WooCommerce didn't show errors.
    </li>
  </ul>
  <p>
    <strong>Version 3.11.0 - 2020.10.09</strong>
  </p>
  <ul>
    <li>New: Support for YITH Composite Products
    </li>
    <li>Improved: Added filter for changing account creation statement: cfw_account_creation_statement
    </li>
    <li>Improved: Fixed some parity issues with complete order process and WooCommerce core. Prevents payment fields from re-initing on submit error.
    </li>
    <li>Improved: Added filters for changing the size of cart thumbnails: cfw_cart_thumb_width, cfw_cart_thumb_height
    </li>
    <li>Fix: Fix issue with body class filter that wasn't returning classes.
    </li>
    <li>Fix: Fix error in Finnish translations.
    </li>
    <li>Fix: Fix JS error when payment field value is null. Fixes Mercado gateway.
    </li>
  </ul>
  <p>
    <strong>Version 3.10.0 - 2020.09.30</strong>
  </p>
  <ul>
    <li>New: Added Express Checkout support for Vipps
    </li>
    <li>Improved: Made it possible for developers to add additional tabs to the checkout process.
    </li>
    <li>Fix: Added margin between shipping packages.
    </li>
    <li>Fix: Added fixes fro SpaSalon theme.
    </li>
    <li>Fix: When license check fails, error is output on the screen.
    </li>
    <li>Fix: Fix issue with NIF Portugal plugin
    </li>
    <li>Fix: Fix issue with WooCommerce Square when an invalid card number is entered.
    </li>
    <li>Fix: Fix issue with PayPal for WooCommerce 2.4.0.
    </li>
  </ul>
  <p>
    <strong>Version 3.9.3 - 2020.09.14</strong>
  </p>
  <ul>
    <li>Developer: Added cfw_after_customer_info_address_heading action
    </li>
    <li>Fix: Fix issue with caching of license activation limit that led to excessive license checks.
    </li>
    <li>Fix: Fix issue where payment request separator "Or" didn't show up with Stripe for WooCommerce.
    </li>
    <li>Fix: Added margin bottom to payment request separator.
    </li>
  </ul>
  <p>
    <strong>Version 3.9.2 - 2020.09.10</strong>
  </p>
  <ul>
    <li>Update tested versions.
    </li>
    <li>Fix: Fix error in Hungarian translations.
    </li>
    <li>Fix: Fix bug that caused Apple Pay / Google Pay to show as active on the payment gateways list with the Glass theme. (Specific to Stripe for WooCommerce - PaymentPlugins)
    </li>
    <li>Fix: Fix issue with YITH Product Bundles that caused bundled items to have editable quantities.
    </li>
    <li>Fix: Fix bug that caused return to shipping link to show up on one page checkout.
    </li>
  </ul>
  <p>
    <strong>Version 3.9.1 - 2020.09.05</strong>
  </p>
  <ul>
    <li>Fix: Fix that super annoying bug in which the phone field setting wasn't honored unless you re-saved it.
    </li>
    <li>Fix: Fix a styling issue with Stripe for WooCommerce payment express buttons.
    </li>
  </ul>
  <p>
    <strong>Version 3.9.0 - 2020.09.01</strong>
  </p>
  <ul>
    <li>New: Compatibility with themes produced by Fuel Themes. Requires latest versions.
    </li>
    <li>Improved: We now sync shipping information to hidden billing fields as they change. This is so that Jilt and similar plugins can correctly get the first and last name information.
    </li>
    <li>Improved: Refactored how we hide / show shipping tab to allow dynamically showing and hiding the shipping tab based on what the cart contains.
    </li>
    <li>Fix: Fix bug where shipping tab was not visible when using 'Hide shipping costs until calculated' option.
    </li>
    <li>Fix: Fixed a couple of PHP notices and warnings.
    </li>
    <li>Fix: Fixed bug with shipping tab when only shipped subscriptions are in the cart.
    </li>
    <li>Fix: Fixed bug with PayPal for WooCommerce not loading the email address correctly on the review page, preventing orders from being submitted.
    </li>
    <li>Fix: Fixed bug with latest version of EU VAT Number that caused field labels to not show up.
    </li>
    <li>Fix: Fix issue where (optional) might show up in promo code field.
    </li>
    <li>Fix: Fix issue with longer payment separator text on mobile devices.
    </li>
  </ul>
  <p>
    <strong>Version 3.8.3 - 2020.08.26</strong>
  </p>
  <ul>
    <li>Fix: Fixed bug where fragments from 3rd party plugins that return non-string values threw JS errors.
    </li>
    <li>Fix: Fixed bug with Germanized for WooCommerce did not pickup billing address during submit.
    </li>
    <li>Fix: Separated logic for showing shipping tab and showing shipping methods to prevent bugs from hidden shipping fields.
    </li>
    <li>Fix: Fixed Dutch translation spelling mistake.
    </li>
    <li>Fix: Fixed bug that caused 'Hide shipping costs until an address is entered' option to hide the shipping tab entirely for stores that don't have a default customer location.
    </li>
  </ul>
  <p>
    <strong>Version 3.8.2 - 2020.08.22</strong>
  </p>
  <ul>
    <li>Hotfix: Fixes critical bug that caused a license check to run on every single page view.
    </li>
  </ul>
  <p>
    <strong>Version 3.8.1 - 2020.08.21</strong>
  </p>
  <ul>
    <li>Hotfix: Fix issue with Authorize.net CIM 3.3.0. (Unrelated to 3.8.0 release)
    </li>
  </ul>
  <p>
    <strong>Version 3.8.0 - 2020.08.21</strong>
  </p>
  <p>
    <strong><u>CheckoutWC 3.8 requires PHP 7.0. If you upgrade on a version prior to 7.0, CheckoutWC functionality will not load.</u></strong>
  </p>
  <ul>
    <li>New: CheckoutWC now requires PHP 7.0.
    </li>
    <li>New: Settings Exporter / Importer
    </li>
    <li>New: User Matching - automatically associate guest orders with existing accounts
    </li>
    <li>New: Support for WooCommerce - Social Login (WPWeb)
    </li>
    <li>New: Support for WooCommerce MailerLite
    </li>
    <li>New: Support for Pont shipping for Woocommerce
    </li>
    <li>New: Added Arabic translations.
    </li>
    <li>Improved: Allow shortcodes in empty cart redirect URL setting.
    </li>
    <li>Improved: Dropped jQuery Migrate from script requirements.
    </li>
    <li>Improved: Checks whether any shipping packages exist when determining whether to show the shipping tab or shipping totals.
    </li>
    <li>Improved: Refactored how we fingerprint payment methods to prevent unnecessary refreshes. Now uses JS just like WooCommerce core.
    </li>
    <li>Improved: Added new filters - cfw_ship_to_label, cfw_cart_totals_shipping_label, cfw_express_pay_separator_text
    </li>
    <li>Fix: Fully working Braintree for WooCommerce (PaymentPlugins) support.
    </li>
    <li>Fix: Fix issue where postal code reverted to wrong value with Square.
    </li>
    <li>Fix: Fix JS error with Ship Mondo.
    </li>
    <li>Fix: Fix issue where default WooCommerce notice wasn't styled correctly.
    </li>
    <li>Fix: Fix bug with WooCommerce style registration that caused an inconsistent state.
    </li>
    <li>Fix: Fix bug that caused enable order notes setting to become unavailable after enabling.
    </li>
    <li>Fix: Fix issue where Klarna Checkout couldn't succeed due to shipping phone field being required.
    </li>
  </ul>
  <p>
    <strong>Version 3.7.4 - 2020.07.30</strong>
  </p>
  <ul>
    <li>Developer: Added cfw_field_data_persistence_excludes filter to allow changing which fields data is persisted on refresh.
    </li>
    <li>Developer: Added cfw_thank_you_title / cfw_thank_you_subtitle filters.
    </li>
    <li>Developer: Added cfw_before_enhanced_login_prompt and cfw_after_enhanced_login_prompt action hooks.
    </li>
    <li>Developer: Added cfw_breadcrumb_cart_url filter.
    </li>
    <li>Developer: Added cfw_shipping_total_address_required_text and cfw_shipping_total_not_available_text filters.
    </li>
    <li>Improved: Trim post code before validating to eliminate issues with trailing spaces.
    </li>
    <li>Improved: Don't call update_checkout until post code field is changed instead of on key down to prevent mid entry error notices.
    </li>
    <li>Improved: Changed 'Not Calculated' notice for shipping calculation to 'Address Required' and 'Not Available' to 'No shipping methods available'
    </li>
    <li>Fix: Fix issues with SkyVerge gateways where a gateway might not set its payment fields correctly.
    </li>
    <li>Fix: Fix issue where express pay buttons didn't load properly on slow sites.
    </li>
    <li>Fix: Fix issues with latest version of EU VAT Number where VAT number field didn't show up
    </li>
    <li>Fix: Fix issue with Elementor Pro header / footer rendering behind cart summary
    </li>
    <li>Fix: Fixed issue with Salient WP Bakery plugin loading CSS that broke the checkout page layout
    </li>
    <li>Fix: Removed duplicate cfw_after_footer hook
    </li>
    <li>Fix: Added back "Order again" button to thank you page
    </li>
    <li>Fix: Fixed bug with Fatture in Cloud compatibility module that caused fields not to render.
    </li>
    <li>Fix: Fix potential bug with Square for slow sites where post code was not set properly.
    </li>
    <li>Fix: Fix logical error with payment gateway fingerprinting that caused payment gateways to never be refreshed on update_checkout AJAX call.
    </li>
  </ul>
  <p>
    <strong>Version 3.7.3 - 2020.07.09</strong>
  </p>
  <ul>
    <li>Improved: Validate email field as email field even if the input type is wrong.
    </li>
    <li>Improved: Added filter to disable editable shipping phone field on order edit screen: cfw_enable_editable_admin_shipping_phone_field
    </li>
    <li>Fix: Fixed missing double quote in cfw_form_field()
    </li>
    <li>Fix: Force select labels for Checkout Add-ons select fields.
    </li>
    <li>Fix: Fix bugs with post code validation when switching countries.
    </li>
    <li>Fix: Fix bugs with Klarna Checkout
    </li>
    <li>Fix: Fix bugs with EveryPay's unique process.
    </li>
    <li>Fix: Run payment request separator handler a little later for slow loading pages.
    </li>
    <li>Fix: Fixes for Square gateway postal code field to prevent it from resetting to wrong value.
    </li>
    <li>Fix: On error during license check, report error to CheckoutWC support and delay license deactivation.
    </li>
    <li>Fix: Fix issue where header and footer were not loaded when Elementor was active, integration was enabled, but didn't have a header or footer set.
    </li>
  </ul>
  <p>
    <strong>Version 3.7.2 - 2020.07.02</strong>
  </p>
  <ul>
    <li>Fix: Fix JS errors in IE 11.&nbsp;
    </li>
    <li>Fix: Fix styling issues with Elementor header / footer and Glass/Copify templates
    </li>
    <li>Fix: Fix issue with Futurist breadcrumb styles
    </li>
    <li>Fix: Fix issue where Elementor being enabled could cause the header and footer not to load on the checkout page.
    </li>
  </ul>
  <p>
    <strong>Version 3.7.1 - 2020.06.23</strong>
  </p>
  <ul>
    <li>Fix: Fix issue where reload command from gateways didn't trigger a page refresh
    </li>
    <li>Fix: Fix issue where Amazon Pay endlessly refreshed
    </li>
    <li>Fix: Fix issue where placeholder for EU VAT Number filed was N/A
    </li>
    <li>Fix: Added back return to cart link on one page checkout
    </li>
    <li>Fix: Fix bug with Beaver Builder header / footer on Glass theme
    </li>
    <li>Fix: Fix issue with PayPal for WooCommerce and billing field required errors
    </li>
    <li>Fix: Fix issue where express checkout area showed up when Mollie Pay is disabled
    </li>
  </ul>
  <p>
    <strong>Version 3.7.0 - 2020.06.19</strong>
  </p>
  <p>
    This is a pretty big release in terms of the number of files changed. We obsessively tested all of the usual use cases and trouble makers and didn't identify any problems, but as always&nbsp; <strong>please test thoroughly on your staging site before updating your live site</strong>&nbsp;to avoid disruptions.
  </p>
  <ul>
    <li>NEW: Support for MolliePay through WooCommerce PensoPay
    </li>
    <li>NEW: Realtime postal code validation. If an invalid postal code is entered during checkout, an error will be immediately displayed. This does not validate that a post code is correct, just that it is a valid postal code for the selected country.
    </li>
    <li>Improved: Added JSON fixing dataFilter from WooCommerce core to complete order hook to try to cover some edge cases where servers send malformed output.
    </li>
    <li>Fix: Fix issue with WooCommerce Service forcing the shipping phone field to be optional.
    </li>
    <li>Fix: Fix issue with Braintree for WooCommerce (PaymentPlugins) PayPal button
    </li>
    <li>Fix: Fix issue where JSON output from AJAX calls encoded arrays as objects.
    </li>
    <li>Fix: Suppress express checkout separator when in final review for PayPal for WooCommerce Express Checkout orders.
    </li>
  </ul>
  <p>
    <strong>Version 3.6.2 - 2020.06.16</strong>
  </p>
  <ul>
    <li>New: When using one page checkout, cart is now position fixed so that it stays visible while scrolling.
    </li>
    <li>New: Added ability to edit the shipping phone on orders in the admin view.
    </li>
    <li>New: Added accent color option for Glass theme to control the color of the shipping options and selected accordion options.
    </li>
    <li>Improved: Shipping options, payment options, and same as shipping toggle now use pointer cursor.
    </li>
    <li>Improved: Allow individually sold products to be removed from the cart when cart editing is active
    </li>
    <li>Fix: Fix issues with Futurist breadcrumbs when skipping shipping option.
    </li>
    <li>Fix: Fix issues with Futurist theme and one page checkout.
    </li>
    <li>Fix: Fix issues with JS validation of fields when one page checkout is enabled.
    </li>
    <li>Fix: Fix issue with Authorize.net and order pay page.
    </li>
    <li>Fix: Use determine_locale() to get the locale instead of using get_user_locale()
    </li>
  </ul>
  <p>
    <strong>Version 3.6.1 - 2020.06.13</strong>
  </p>
  <ul>
    <li>Hotfix: Fix issue with WooCommerce Gift Cards and the mobile coupon feature.
    </li>
  </ul>
  <p>
    <strong>Version 3.6.0 - 2020.06.12</strong>
  </p>
  <p>
    This is a pretty substantial update. There shouldn't be any breaking changes, however&nbsp; <strong>please test before upgrading your live site.</strong>
  </p>
  <ul>
    <li>NEW: One Page Checkout option. When enabled, the three steps become one longer step. Useful for digital stores.
    </li>
    <li>NEW: Beaver Themer support. Use Beaver Themer to build custom headers and footers and override the header and footer on the checkout page.
    </li>
    <li>NEW: Experimental Integration - Template Loader. This feature allows you to load the checkout template inside your WordPress theme. This option is unsupported, so you'll need to be prepared to deal with any styling issues that may result.
    </li>
    <li>NEW: Added support for WooCommerce Advanced Messages
    </li>
    <li>NEW: Added support for ShipIt / WooCommerce Carrier Agents
    </li>
    <li>NEW: Added support for the Tokoo theme
    </li>
    <li>NEW: Added support for the Stokie theme
    </li>
    <li>Improved: Added support for express payment buttons for Stripe for WooCommerce (PaymentPlugins)
    </li>
    <li>Fix: Fix issue with WooCommerce Order Delivery Date
    </li>
    <li>Fix: Attempt to fix issue with CSS animations and artifacts in Safari
    </li>
    <li>Fix: Fix issue with PayPal for WooCommerce smart button not displaying after toggling billing address.
    </li>
  </ul>
  <p>
    <strong>Version 3.5.6 - 2020.06.10</strong>
  </p>
  <ul>
    <li>Fix - Fix issue with invalid post code message and Square (official) gateway
    </li>
    <li>Fix - Add English (UK) translations as some people might need them.
    </li>
    <li>Fix - Add back missing order totals on order pay page.
    </li>
  </ul>
  <p>
    <strong>Version 3.5.5 - 2020.06.09</strong>
  </p>
  <ul>
    <li>Fix - Fix issue with PayPal for WooCommerce and express checkout where confirmation page didn't appear.
    </li>
    <li>Fix - Fix issue with WooCommerce Price Based on Country.
    </li>
    <li>Fix - Fix issue where currency formats that include spaces resulted in prices wrapping to the next line.
    </li>
  </ul>
  <p>
    <strong>Version 3.5.4 - 2020.06.05</strong>
  </p>
  <ul>
    <li>Fix - Fix issues with Barberry theme (specifically the Barberry Extension plugin)
    </li>
    <li>Fix - Fix issue with terms and conditions on order pay page
    </li>
    <li>Fix - Fix field layout for Brazilian Market for WooCommerce plugin
    </li>
    <li>Fix - Fix translation strings from WooCommerce core that have changed.
    </li>
  </ul>
  <p>
    <strong>Version 3.5.3 - 2020.06.04</strong>
  </p>
  <ul>
    <li>Hotfix - Fix issue with WooCommerce 4.2 that caused the row containing country, post code, and state to be invisible when either switching to a country that has no states or loading the checkout page with a country that has no states.
    </li>
  </ul>
  <p>
    <strong>Version 3.5.1 - 2020.06.03</strong>
  </p>
  <ul>
    <li>Fix - Fix issue where WooCommerce Square (official gateway) postal code field wasn't updated when the 'Same as shipping address' radio was toggled or the billing postcode was changed.
    </li>
    <li>Fix - Firm up styles on field rows to prevent themes or plugins from messing with them.
    </li>
    <li>Fix - Add more specificity to the checkmark styles on the thank you page to prevent themes or plugins from messing with them.
    </li>
  </ul>
  <p>
    <strong>Version 3.5.0 - 2020.05.31&nbsp;</strong>
  </p>
  <p>
    There are some pretty substantial changes here.&nbsp; <strong>Please test before deploying to your live site.</strong>
  </p>
  <ul>
    <li>NEW: Mobile Coupon field. Show a separate coupon field on mobile so that customers don't have to hunt for it. (Optional)
    </li>
    <li>NEW: Refactored how our tab system transitions between tabs to fix issues with gateways that use iframes. This is actually a huge performance bonus as we no longer have to selectively refresh for certain gateways like Square, Cybersource, etc.
    </li>
    <li>NEW: Support for TheBox theme.
    </li>
    <li>Improved: Added eslint and cleaned up our JS files.
    </li>
    <li>Improved: Added a new filter:&nbsp;cfw_transactions_encrypted_statement
    </li>
    <li>Fix: Fixed issue where Authorize.net card logo watermark didn't appear.
    </li>
    <li>Fix: Fix margin on PayPal Express button.
    </li>
    <li>Fix: Fix issue where state wasn't properly filled when using Address Autocomplete.
    </li>
    <li>Fix: Fix issue with PayPalPlus and coupons.
    </li>
    <li>Fix: Fix bug with Klarna Checkout that caused an endless redirect loop.
    </li>
    <li>Fix: Fix bug with YITH Order Delivery Date.
    </li>
  </ul>
  <p>
    <strong>Version 3.4.2 - 2020.05.22</strong>
  </p>
  <ul>
    <li>Hotfix: Fix issue where Square CC fields didn't load properly.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 3.4.1 - 2020.05.22</strong>
  </p>
  <ul>
    <li>Fix: Fix issue where checkout page scrolled strangely on iPhone.
    </li>
    <li>Fix: Fix issue where WP admin bar didn't position correctly on mobile devices.
    </li>
  </ul>
  <p>
    <strong>Version 3.4.0 - 2020.05.21</strong>
  </p>
  <ul>
    <li>NEW: Refactored how we refresh the checkout page to minimize the number of times it happens. This should make the checkout page much nicer to interact with and save a lot of server CPU cycles.&nbsp;
    </li>
    <li>NEW: Added option to skip shipping step for stores with one shipping option.
    </li>
    <li>NEW: Added support for WooCommerce Gift Cards (Official)
    </li>
    <li>Improved: We no longer block the next tab buttons during refreshes.
    </li>
    <li>Fix - Fixed bug with show mobile credit card logos option.
    </li>
    <li>Fix - Fixed bug with JupiterX theme.
    </li>
    <li>Fix - Fixed bug where opting in to stat collection double tracked stats.
    </li>
    <li>Fix - Fixed bug with NL Postcode Checker.
    </li>
    <li>Fix - Fixed bug with PostNL
    </li>
    <li>Fix - Removed warning for&nbsp;Checkout Field Editor for WooCommerce by ThemeHigh since customers have confirmed it works now.
    </li>
    <li>Fix - Fix styling bug with quantity steppers and IE11.
    </li>
    <li>Fix - Fix bug where clicking on promo field on phones zoomed in.
    </li>
    <li>Fix - Fix potential fatal error with Amazon Pay.
    </li>
    <li>Fix - Fix bug where save card checkbox was visible when a customer opted to not create an account.
    </li>
    <li>Fix - Fix styling bug with third party plugin checkboxes.
    </li>
  </ul>
  <p>
    <strong>Version 3.3.0 - 2020.05.07</strong>
  </p>
  <ul>
    <li>NEW: By popular request, the cart editing controls have been replaced with a quantity stepper.
    </li>
    <li>NEW: Added option to control whether thank you page template is used when viewing orders in My Account.
    </li>
    <li>NEW: Added option to show credit card logos on mobile.
    </li>
    <li>Improved: Added console logging when an unknown server response is sent during complete order.
    </li>
    <li>Improved: Added filename to downloads list.
    </li>
    <li>Improved: Moved password above create account checkbox instead of below. (Only applies option to allow customers to set a password is used)
    </li>
    <li>Fix: Fix bug where change log doesn't show up properly.
    </li>
    <li>Fix: Fix bug with newest version of Square gateway (confirmed to work with 2.1.4)
    </li>
    <li>Fix: Fix bug with YITH Order Delivery Date integration.
    </li>
    <li>Fix: Fix bug with PayPal for WooCommerce that resulted in an error about billing email being a required field.
    </li>
    <li>Fix: Fix overlay position during order submit. Now covers whole viewport and spinner will always be centered.
    </li>
    <li>Fix: Fix bug with Futurist theme and breadcrumb width on mobile.
    </li>
    <li>Fix: Fix bug where 'Allow stat collection' notice didn't actually enable stat collection.
    </li>
    <li>Fix: Fix whitespace on the right side of screen on iPhone.
    </li>
    <li>Fix: Fix issue with Braintree for WooCommerce by PaymentPlugins where error messages weren't shown.
    </li>
    <li>Fix: Fix issue where Authorize.net saved cards didn't show up properly on order pay page.
    </li>
    <li>Fix: Fix bug where conflicting styles could cause the Amazon Pay express button to have text beneath it.
    </li>
    <li>Fix: Fix bug where JS validation error messages were not translated into Greek.
    </li>
  </ul>
  <p>
    <strong>Version 3.2.0 - 2020.05.01</strong>
  </p>
  <ul>
    <li>New: Added Express checkout support for Braintree for WooCommerce by PaymentPlugins.
    </li>
    <li>New: Added support for WooCommerce Product Bundles.
    </li>
    <li>New: Greek translations.
    </li>
    <li>Improved: Added cfw_payment_method_address_review_shipping_method filter.
    </li>
    <li>Improved: Eliminated closures in template-hooks.php for easier unhooking.
    </li>
    <li>Improved: Added compatibility mode filter for sites that load Google Maps from another location: cfw_google_maps_compatibility_mode
    </li>
    <li>Improved: Added cfw_cart_item_row_class filter.
    </li>
    <li>Fix: Fix issues with WooCommerce style registration setup.
    </li>
    <li>Fix: Make sure cfw-customer-info-active is active on form on page load.
    </li>
    <li>Fix: Fix endless redirect bug with Klarna Checkout.
    </li>
    <li>Fix: Multiple fixes for Amazon Pay.
    </li>
    <li>Fix: Fix bug with multiple payment gateways on the order pay page, including Sezzle and PostFinance.
    </li>
    <li>Fix: Fix issue with quotes in blog name.
    </li>
    <li>Fix: Add noncing back to update checkout call. Fixes issue with plugin that expects it.
    </li>
  </ul>
  <p>
    <strong>Version 3.1.0 - 2020.04.26</strong>
  </p>
  <ul>
    <li>New: Added support for Upsell Order Bump Offer.
    </li>
    <li>New: Added official fix for Pimwick Gift Cards Pro. Adds gift card field under the coupon code field.
    </li>
    <li>Fix: Added back cfw_after_cart_summary hook.
    </li>
  </ul>
  <p>
    <strong>Version 3.0.5 - 2020.04.21</strong>
  </p>
  <ul>
    <li>Fix: Fix bug with PayPal for WooCommerce and the final review screen for logged out users.
    </li>
    <li>Fix: Fix bug with latest version of Amazon Pay that caused the address fields to be hidden.
    </li>
    <li>Fix: Cleaned up locale code for field validation translations.
    </li>
    <li>Fix: Added support for getting the Weglot current locale for field validation translations.
    </li>
    <li>Fix: Fix translation of 'Contact' in Portuguese translations.
    </li>
  </ul>
  <p>
    <strong>Version 3.0.4 - 2020.04.16</strong>
  </p>
  <ul>
    <li>Improved: We now hide the WooCommerce Account setting for generating account passwords depending on your Registration Style setting.
    </li>
    <li>Improved: We now override and hide the WooCommerce Account setting for generating usernames since this should always be true for CheckoutWC.
    </li>
    <li>Fix: Fix multiple bugs with Amazon Pay.
    </li>
    <li>Fix: Fix WooCommerce warning when using Amazon Pay with PayPal for WooCommerce
    </li>
    <li>Fix: Fix potential fatal error.
    </li>
    <li>Fix: Fix bug with WooCommerce Local Pickup Plus.
    </li>
  </ul>
  <p>
    <strong>Version 3.0.3 - 2020.04.14</strong>
  </p>
  <ul>
    <li>Improved: Replace jQuery(document).ready with a lighter replacement that is more error tolerant. This makes CheckoutWC more tolerant of errors from 3rd party scripts.
    </li>
    <li>Improved: Added 67% field width option to WooCommerce Checkout Field Editor.
    </li>
    <li>Fix: Fix issue where Square gateway no loner re-ordered the payment tab to place the billing address before the credit card fields.
    </li>
    <li>Fix: Fix issue where the window did not scroll to the top properly when multiple notices were added in quick succession.
    </li>
  </ul>
  <p>
    <strong>Version 3.0.2 - 2020.04.11</strong>
  </p>
  <ul>
    <li>Fix: Fix issue where System Font Stack setting was being saved in a translated state, which broke fonts on the page.
    </li>
    <li>Fix: Fix MailChimp for WooCommerce checkbox styles.
    </li>
    <li>Fix: Fix issue where size options for WooCommerce Checkout Field Editor weren't showing up.
    </li>
    <li>Fix: Improve handling of built in form-row-first and form-row-last classes so that it uses a proper grid wrap. Fixes mobile styling of Authorize.net field gateways, etc.
    </li>
  </ul>
  <p>
    <strong>Version 3.0.1 - 2020.04.11</strong>
  </p>
  <ul>
    <li>Fix: Fix untranslated strings.
    </li>
    <li>Fix: Order admin bar menu same as the tabs in settings.
    </li>
    <li>Fix: Add updated support tab that was removed during a merge.
    </li>
    <li>Fix: Firm up background color to prevent plugins / themes from messing with it.
    </li>
    <li>Fix: Handle long label lengths for 'Ship to' in shipping address preview on shipping method and payment tabs.
    </li>
    <li>Fix: Change 'Shipping method' to 'Method' so that labels are shorter.
    </li>
  </ul>
  <p>
    <strong>Version 3.0.0 - 2020.04.10</strong>
  </p>
  <p>
    <strong>This is a major version update. Please test before updating your live site. If you're using a custom CheckoutWC template, do NOT update. You will need to rebuild your template.&nbsp;</strong>
  </p>
  <ul>
    <li>NEW: A brand new theme (Glass) for a brand new version (3.0!)
    </li>
    <li>NEW: Added options for the most common customizations. Control Order Notes, Cart Item options, Login and Registration right from settings.
    </li>
    <li>NEW: Reorganized admin screens to make finding things easier.
    </li>
    <li>NEW: Refactored templates to use action hooks.
    </li>
    <li>NEW: Refactored JS and CSS to be more modular and less coupled.
    </li>
    <li>NEW: Added support for Russian, Slovakian, and Japanese.
    </li>
    <li>NEW: Added support for CartFlows. You can control whether CheckoutWC loads a checkout step right from the step settings.
    </li>
    <li>NEW: More robust grid framework with better mobile responsive styles.
    </li>
    <li>NEW: Redesigned cart summary with better data display, quantity bubbles (similar to Shopify) and cart editing.
    </li>
    <li>NEW: Dynamic field resizing when switching between countries.
    </li>
    <li>NEW: Built in support for Google Fonts.
    </li>
    <li>NEW: More design options: set the body background color, text color, hover colors, and more.
    </li>
    <li>NEW: Added Shopify style preview above each step summarizing the choices made in previous steps.
    </li>
    <li>NEW: Added Weglot support.
    </li>
    <li>NEW: Support for PayPal for WooCommerce final review page.
    </li>
    <li>NEW: Option to use traditional rather than floating labels.
    </li>
    <li>NEW: When migrating your site, the stats opt-in setting will automatically turn off until you re-enable it.
    </li>
    <li>FIX: Fixed bugs with Klarna Checkout 2.x
    </li>
    <li>FIX: Fixed some Finnish translations.
    </li>
    <li>And much more! This release includes 243 commits and includes lots of little tweaks, improvements, and enhancements.
    </li>
  </ul>
  <p>
    <strong>Version 2.44.0 - 2020.03.05</strong>
  </p>
  <ul>
    <li>New: Added support for YITH Delivery Date.
    </li>
    <li>New: Added code editor to header / footer scripts and custom CSS.
    </li>
    <li>New: On activation, we now set the logo from your WordPress customizer settings if it isn't already set.
    </li>
    <li>New: Added custom text area to thank you page template. Use action: cfw_thank_you_text. This renders above Order Updates.
    </li>
    <li>Improved: Better parsing of error messages that are added to the page with JavaScript.
    </li>
    <li>Improved: Added reminder when CheckoutWC is licensed and activated but not enabled.
    </li>
    <li>Improved: JS and CSS assets are now output with the version number in the filename. This busts cache automatically even when using plugins that remove version number query strings.
    </li>
    <li>Improved: Changed default colors to be more neutral.
    </li>
    <li>Fix: Fixed a few issues with Amazon Pay.
    </li>
    <li>Fix: Fixed a few issues with Genesis theme.
    </li>
    <li>Fix: Fixed a few styling issues that happen when bootstrap styles are present on the page.
    </li>
    <li>Fix: Templates now have independent webpack configs to make custom development easier. (But don't start any custom templates until version 3.0 is released!)
    </li>
    <li>Fix: Fixed bug that prevented express pay buttons from showing up if you refreshed the page on a tab other than customer information.
    </li>
    <li>Fix: Fixed bug with thank you page that prevented order status from rendering properly for unshipped orders.
    </li>
    <li>Fix: Fixed bug where Apple Pay did not show up with Stripe gateway.
    </li>
    <li>Fix: Fixed bug where New Zealand states did not populate with address autocomplete enabled.
    </li>
  </ul>
  <p>
    <strong>Version 2.43.2 - 2020.02.17</strong>
  </p>
  <ul>
    <li>Fix: Refactor how we handle showing / hiding the shipping method tab to fix issues with WooCommerce Subscriptions.
    </li>
    <li>Improved: Added alert styling to the 'There are no shipping methods available' message.
    </li>
    <li>Improved: Fixed styling issues with WooCommerce Subscription shipping methods.
    </li>
    <li>Improved: Improved how we parse error messages during checkout submit to squash some edge cases.
    </li>
    <li>Fix: Fix bug where error messages had bullet point styling.
    </li>
    <li>Fix: Fix issue with Swedish translations not working in all cases.
    </li>
    <li>Updated WooCommerce tested version to 3.9.1
    </li>
  </ul>
  <p>
    <strong>Version 2.43.1 - 2020.02.17</strong>
  </p>
  <ul>
    <li>Hotfix: Fixed express checkout wrapper showing up even when no express buttons are available.
    </li>
  </ul>
  <p>
    <strong>Version 2.43.0 - 2020.02.14</strong>
  </p>
  <ul>
    <li>New: Payment buttons now have a wrapper similar to Shopify's that says 'Express checkout': <a href="https://www.dropbox.com/s/9s7ertyxkjnkmwc/Screenshot%202020-02-14%2016.09.54.png?dl=0">https://www.dropbox.com/s/9s7ertyxkjnkmwc/Screenshot%202020-02-14%2016.09.54.png?dl=0</a>
    </li>
    <li>Improved: State dropdown now default to 'Select an option'. This is necessary because default geolocation no longer includes state.
    </li>
    <li>Improved: Added Swedish translations.
    </li>
    <li>Fix bug with Konte theme.
    </li>
    <li>Fix NextGen Gallery bug for real this time.
    </li>
    <li>Fix submit on enter bug with Safari.
    </li>
    <li>Fix overlay position bug.
    </li>
    <li>Handle custom quantities 10 and over with cart editing better.
    </li>
    <li>Switch cart list HTML to a table so we can style it more consistently.
    </li>
    <li>Fix padding on cart for Copify theme.
    </li>
    <li>Fix bug with recent versions of Checkout Add-ons.
    </li>
    <li>Fix PHP warning with constants and the Copify theme.
    </li>
    <li>Fix bug in thank you page template that didn't display the map when shipping address forced to the billing address.
    </li>
    <li>Fix bug where viewing an order that has items that no longer exists resulted in a fatal error.
    </li>
    <li>Fix styling issues with themes by hardening some of our styles.
    </li>
    <li>Fix styling bug with postal code field that caused it to appear shorter than surrounding fields.
    </li>
    <li>Fix bug where Finnish translations did not work properly.
    </li>
    <li>Fix bug with Square where error messages repeated and were unstyled.
    </li>
  </ul>
  <p>
    <strong>Version 2.42.0 - 2020.02.08</strong>
  </p>
  <ul>
    <li>New: Support for <a href="https://www.checkoutwc.com/documentation/permit-elementor-styles-and-scripts-on-the-checkout-page">Elementor Pro!</a>
    </li>
    <li>New: Support for WPC Product Bundles
    </li>
    <li>New: Compatibility with Blaszok theme
    </li>
    <li>Improved Portuguese translations.
    </li>
    <li>Improved Italian translations.
    </li>
    <li>Improved styling of cart item meta data on checkout and thank you pages.
    </li>
    <li>Workaround major bug in latest version of NextGen Gallery that prevented our AJAX hooks from returning data.
    </li>
    <li>Fix bug with placeholders and Safari credit card autocomplete.
    </li>
    <li>Fix JS errors when Google Maps script isn't loaded and autocomplete is enabled.
    </li>
    <li>Fix visual glitch with select fields that fail validation.
    </li>
    <li>Fix issue where breadcrumb tab navigation didn't show up for Copify theme on mobile.
    </li>
    <li>Fixed a PHP notice.
    </li>
    <li>Fix bug with PayPalPlusCw
    </li>
    <li>Fix issue where WooCommerce fields were being wrapped with our markup on non-checkout pages.
    </li>
  </ul>
  <p>
    <strong>Version 2.41.3 - 2020.01.26</strong>
  </p>
  <ul>
    <li>Fix issues with Portuguese and Finnish translations.&nbsp;
    </li>
    <li>Fix issue with NL Postcode Checker.
    </li>
    <li>Fix issue with WooCommerce 3.9 notices showing up as "Array".
    </li>
    <li>Fix issue where order pay page didn't show error message with Copify template.
    </li>
    <li>Improved: Split JS files into 2 to reduce load size of each file.
    </li>
  </ul>
  <p>
    <strong>Version 2.41.2&nbsp;- 2020.01.20</strong>
  </p>
  <ul>
    <li>Fix bug with Portugal VASP Kios
    </li>
    <li>Fix bug where hidden submit button could be made visible by other plugins.
    </li>
  </ul>
  <p>
    <strong>Version 2.41.1 - 2020.01.18</strong>
  </p>
  <ul>
    <li>Updated translation files.
    </li>
    <li>Updated the way variation data is showed under cart items to better support long and complicated output.
    </li>
    <li>Fixed bug where cart is not cleared on successful order when using thank you page feature.
    </li>
    <li>Fixed bug where processing overlay / animation were not removed when checkout fails for gateways like Klarna Payments.
    </li>
    <li>Fixed bug where Polish and Portuguese translations were not loaded for some derivations of those languages.
    </li>
    <li>Fixed bug that caused gateway fields to reset when changing billing address toggle.
    </li>
  </ul>
  <p>
    <strong>Version 2.41.0 - 2020.01.13</strong>
  </p>
  <ul>
    <li>Added support for Portugal VASP Kios plugin.
    </li>
    <li>Added support for WooCommerce Advanced Shipment Tracking
    </li>
    <li>Added filter to allow overriding login failed error message: cfw_failed_login_error_message
    </li>
    <li>Prevent LastPass from monkeying around with Google API key field in settings.
    </li>
    <li>Fix issue that prevented Facebook Messenger chat from showing up.
    </li>
    <li>Fixed some PHP notices.
    </li>
    <li>Fix issue with where Jilt renders it's consent checkbox.
    </li>
    <li>Fix issue where paid to free and back switches weren't working properly.
    </li>
    <li>Fix issue with forcing WooCommerce to use billing address for billing and shipping.
    </li>
    <li>Fix issue with latest versions of PayPal for WooCommerce.
    </li>
    <li>Fix issue where register checkbox was not available when disabling the login reminder.
    </li>
    <li>Fix mobile styling issues with some payment gateways.
    </li>
    <li>Fix bug with WooFunnels Order Bump rendering the bumps twice.
    </li>
    <li>Fix bug on the thank you page that rendered the cart total on mobile instead of the order total.
    </li>
    <li>Fix styling bug on Copify theme for mobile.
    </li>
    <li>Fix bug where checkout form tries to submit when pressing enter in a field.
    </li>
  </ul>
  <p>
    <strong>Version 2.40.2 - 2019.12.31</strong>
  </p>
  <ul>
    <li>Hotfix for fatal error with some configurations that use woocommerce_after_shipping_rate hook.
    </li>
  </ul>
  <p>
    <strong>Version 2.40.0&nbsp;- 2019.12.18</strong>
  </p>
  <p>
    Happy Holidays! We slowed our normal release schedule to minimize problems throughout the holiday sales cycle. But we have been hard at work on a big update.&nbsp;
  </p>
  <p>
    This update includes a few refactors and while we have obsessively tested the changes, <strong>your store is different than ours!</strong>
  </p>
  <p>
    <strong>Before updating your live site, PLEASE TEST THOROUGHLY.</strong> We don't want any of our customers to lose sales during this important season.
  </p>
  <ul>
    <li>New: You can now use Checkout Field Editor to modify your billing and shipping address fields. We still think most stores should leave this alone, but this makes it much easier to add custom address fields. We also <a href="https://www.checkoutwc.com/documentation/how-to-add-a-custom-field">updated our documentation</a>. This is disabled by default to prevent issues with existing stores.
    </li>
    <li>New: Added support for&nbsp;NIF (Num. de Contribuinte PortuguÃªs) for WooCommerce
    </li>
    <li>New: Added support for WooCommerce Order Delivery.
    </li>
    <li>Improved: If license is detected as inactive, we do an additional check when loading the checkout page to reduce the chance of a false positive.
    </li>
    <li>Improved: Refactored template files to use action hooks to queue the different sections. This makes it easier to maintain the template files and also makes it easier to reorder the layout of each tab without using a custom template.
    </li>
    <li>Improved: Added filters to allow tracking numbers to be added to the thank you page without using WooCommerce Shipment Tracking. Filter:&nbsp;cfw_thank_you_tracking_numbers
    </li>
    <li>Improved: Added better support for WooCommerce Local Pickup Plus
    </li>
    <li>Improved: Changed license check settings to not use an autoloaded WordPress option.
    </li>
    <li>Improved: Styles for 2Checkout
    </li>
    <li>Improved: Added filter to allow bypassing CheckoutWC templates. Filter:&nbsp;cfw_bypass_templates
    </li>
    <li>Improved: Order again button now appears on thank you page.
    </li>
    <li>Fixed issue where download links for digital orders did not appear on thank you page.
    </li>
    <li>Fixed issues with Amazon Pay. Create account process now works like WooCommerce native checkout.
    </li>
    <li>Fixes for issues with Amazon Pay and digital orders.
    </li>
    <li>Fixed issues with Amazon Pay and Subscription orders. When purchasing a subscription, the 'Address preview' on the shipping method tab is hidden. This is due to a currently unsolvable problem that prevents us from looking up the customers selected address accurately.
    </li>
    <li>Fixed issue with Webshipper.
    </li>
    <li>Fixed styling issues on mobile.
    </li>
    <li>Fixed issues with Hebrew language and admin settings page.
    </li>
    <li>Fixed issue with invisible checkbox fields and WooCommerce Checkout Field Editor.
    </li>
    <li>Fix - Removed #cart hash from cart link.
    </li>
  </ul>
  <p>
    <strong>Version 2.39.3 - 2019.11.18</strong>
  </p>
  <ul>
    <li>New: PayPalPlusCw gateway support.
    </li>
    <li>Improved: Added cfw_thank_you_after_cart_summary action to thank you templates.
    </li>
    <li>Improved: Strip out some unnecessary data from update checkout, etc calls that could trigger antivirus software heuristic scanners to block dynamic updates.
    </li>
    <li>Fix: Block CSS hero from loading their CSS on the checkout page.
    </li>
    <li>Fix: Don't try to show empty WooCommerce notices.
    </li>
    <li>Fix: Fix bug with latest Avada version.
    </li>
    <li>Fix: Fix issue with Klarna Payments update.
    </li>
    <li>Fix: Fix bug where extra HTML in Copify sidebar didn't show up without special CSS.
    </li>
    <li>Fix: Thank you page now shows formatted order number instead of internal ID.
    </li>
  </ul>
  <p>
    <strong>Version 2.39.2 - 2019.11.07</strong>
  </p>
  <ul>
    <li>New: Support for Fattureincloud for WooCommerce
    </li>
    <li>Improved: Added cfw_before_thank_you_customer_information filter and added $order object to all filters / actions on the checkout page.
    </li>
    <li>Fix: Fix issue with Avada and thank you page.&nbsp;
    </li>
    <li>Fix: Fix issue with Avada image lazy loading and checkout / thank you pages.
    </li>
  </ul>
  <p>
    <strong>Version 2.39.1 - 2019.11.06</strong>
  </p>
  <ul>
    <li>Improved: Made it possible to change the billing address location without breaking stuff.
    </li>
    <li>Fix: Fix issue where Oxygen Builder output conflicting styles on the checkout page.
    </li>
    <li>Fix: Fix issue where Stripe separator showed up even when no payment buttons were available.
    </li>
    <li>Fix: Fix issue where down arrow on select elements was not clickable.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.39.0 - 2019.11.06</strong>
  </p>
  <ul>
    <li>ðŸŽ‰&nbsp;NEW PREMIUM FEATURE: Thank You Page - This highly requested feature allows you to replace your ugly WooCommerce thank you page with a Shopify style thank you page, complete with map embedding. <a href="https://www.checkoutwc.com/documentation/how-to-enable-and-configure-the-thank-you-page">Details here.</a>
    </li>
    <li>Improved: Added filters for every return / continue button.
    </li>
    <li>Improved: Strengthened field styles to prevent other plugins from messing with them.
    </li>
    <li>Improved: Moved all premium features to their own section in General settings.
    </li>
    <li>Fix: Fix bug with PayPal for WooCommerce final review page.
    </li>
    <li>Fix: Fix JS errors when Google maps doesn't load properly.&nbsp;
    </li>
    <li>Fix: Fix PHP notices.
    </li>
  </ul>
  <p>
    <strong>Version 2.38.3 - 2019.10.26</strong>
  </p>
  <ul>
    <li>Fix: Fix issues with Chronopost
    </li>
    <li>Fix: Fix issues with JupiterX theme and JupiterX Core plugin
    </li>
    <li>Improved: Added Hebrew translations
    </li>
  </ul>
  <p>
    <strong>Version 2.38.2 - 2019.10.23</strong>
  </p>
  <ul>
    <li>New: Add support for Order Delivery Date Lite.
    </li>
    <li>Improved: Alerts from pickup point shipping providers are now temporary and are removed when advancing tabs successfully.
    </li>
    <li>Fix: Fix a few asymptomatic bugs with our tabbing system after the refactor.
    </li>
    <li>Fix: Fix bug where Braintree payment fields did not load after compatibility module loader refactor.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.38.1 - 2019.10.21</strong>
  </p>
  <ul>
    <li>Fix: Fix bug where it was impossible to go to payment when a digital product is in the cart with SendCloud and ShipMondo.
    </li>
    <li>Fix: Fix bug where JS errors happened when Klarna Checkout was activated.
    </li>
  </ul>
  <p>
    <strong>Version 2.38.0 - 2019.10.20</strong>
  </p>
  <ul>
    <li>New: Add support for Inpsyde PayPal Plus gateway.&nbsp;
    </li>
    <li>New: Added ability to use native WooCommerce login form with new filter: cfw_suppress_default_login_form
    </li>
    <li>New: Support for Woo Square Pro.
    </li>
    <li>New: Add ability to ask users for custom password.
    </li>
    <li>Improved: Refactored tab switching code to clean up some ugly workarounds.
    </li>
    <li>Improved: Refactored JS compatibility factory.
    </li>
    <li>Improved: Bypass flag is now comprehensive. <a href="https://www.checkoutwc.com/documentation/how-to-bypass-checkoutwc-for-testing">More info.</a>
    </li>
    <li>Fix: Fix edge case bug where PHP fatal error was possible with PayPal Checkout in one install.
    </li>
    <li>Fix: Fix translation of 'Remove Item'
    </li>
    <li>Fix: Fix deprecation warning
    </li>
    <li>Fix: Fix bug with WooCommerce 3.8.0 RC 1
    </li>
    <li>Fix: Fix ShipMondo issue with modal. Add error message to prevent going to payment without selecting pickup point.
    </li>
    <li>Fix: Fix SendCloud tab advance protection bug.
    </li>
    <li>Fix: Add translation to messages from shipping pickup point plugins that need to prevent advancing to payment before selecting a pickup point.
    </li>
    <li>Fix: Fixed breadcrumb label filter typo.
    </li>
    <li>Fix: Spinner is now centered to viewport during checkout submission.
    </li>
    <li>Fix: Fix bug with Checkout Add-ons and multi-select. All selects from Checkout Add-ons now use Select2.
    </li>
    <li>Fix: Fix bug where scroll to error messages and top of tabs did not fire.
    </li>
  </ul>
  <p>
    <strong>Version 2.37.1 - 2019.10.05</strong>
  </p>
  <ul>
    <li>Fix: Fix bug with Futurist breadcrumb.
    </li>
    <li>Fix: Fix bug where states did not populate when switching countries.
    </li>
    <li>Fix: Prevent 'undefined' text in address field when using Google Maps Address Autocomplete.
    </li>
    <li>Fix: Remove field validation errors when autocompleting state / city from post code.
    </li>
    <li>Fix: Fix issue with PixelYourSite Pro.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.37.0 - 2019.09.29</strong>
  </p>
  <ul>
    <li>New: Support for Electro theme.
    </li>
    <li>New: In3 gateway support.
    </li>
    <li>New: WooCommerce Subscription Gifting support.
    </li>
    <li>Improved: Lots of fixes for Checkout Add-ons 2.x
    </li>
    <li>Improved: Add filters for breadcrumbs.&nbsp;
    </li>
    <li>Improved: Fixed issues with moving order button on order pay page for German stores.
    </li>
    <li>Fix: Catch relative protocol theme styles / scripts.&nbsp;
    </li>
    <li>Fix: Fix issue with low stock quantities and cart editing dropdown.
    </li>
    <li>Fix: Fix issue with add to cart notices on checkout. Added filter to conditionally show these notices when desired.
    </li>
    <li>Fix: Fix checkbox label text sizes to be more consistent.
    </li>
    <li>Fix: Style links properly according to color in settings.
    </li>
    <li>Fix: Alerts that are present on checkout page load will now persist until a subsequent update checkout AJAX call.
    </li>
    <li>Fix: SendCloud now requires picking a pickup point before advancing to the next section.
    </li>
    <li>Fix: Cleaned up some potential PHP warnings.&nbsp;
    </li>
    <li>Fix: Fixed bug with Order Delivery Date and PayPal Checkout that could cause an endless update loop.
    </li>
  </ul>
  <p>
    <strong>Version 2.36.1 - 2019.09.19</strong>
  </p>
  <ul>
    <li>Hotfix: The last update inadvertently applied our Avada workarounds on every page instead of the checkout page. We're really sorry about this. This update fixes the problem.
    </li>
  </ul>
  <p>
    <strong>Version 2.36.0 - 2019.09.17</strong>
  </p>
  <ul>
    <li>New: For stores that require registration, we now prevent continuing to the shipping method if we detect that your email address matches an account and that you haven't logged in.&nbsp;
    </li>
    <li>Improved: Allow fee only orders with order pay page.&nbsp;
    </li>
    <li>Improved: Switch product thumbnails to use new cfw_cart_thumbnail image size so that smaller images are loaded. (Requires <a href="https://www.wpbeginner.com/plugins/regenerate-thumbnails-new-image-sizes-wordpress/">regeneration of thumbnails</a>to fully take advantage)
    </li>
    <li>Improved: Added more filters to allow overriding headings and label.
    </li>
    <li>Improved: When using zip autocomplete, we only fill in the city if there's only one possible match. This provides a better user experience when we can't be certain which city is the actual match.
    </li>
    <li>Improved: When using the setting 'Force shipping to the customer billing address' the address heading is now 'Billing and Shipping address'
    </li>
    <li>Fix: Fix bug with 3D Secure failures and Stripe.
    </li>
    <li>Fix: Fix bug where Avada snuck in a lot of breaking CSS.
    </li>
    <li>Fix: Fix bug where mobile total didn't update.&nbsp;
    </li>
    <li>Fix: Fix bug where countries that don't require postal code didn't allow continuing to next screen.
    </li>
    <li>Fix: Fix bug with Divi that hid the contents of the shipping address tab.
    </li>
    <li>Fix: Fix bug where products without inventory tracking didn't have the proper quantity options when using cart editing.
    </li>
    <li>Fix: Rollback whitespace change to totals that caused subscription prices to run continuously off of the page. If you need to prevent whitespace wrapping, you'll need to do this with custom CSS.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.35.0 - 2019.09.06</strong>
  </p>
  <ul>
    <li>Improved: Added filter cfw_header_home_url to allow changing the home URL link in the header. <a href="https://www.checkoutwc.com/documentation/how-to-change-the-header-link-url">More information.</a>
    </li>
    <li>Improved: Added the ability to adjust cart item quantity over 10. It now prompts the user to enter their desired quantity when selecting '10+'.&nbsp;
    </li>
    <li>Improved: Re-factored how alerts are handled to make them more consistent / standardized.&nbsp;
    </li>
    <li>New: Support for Flevr theme
    </li>
    <li>Fix: Fix bug where form field persistence library emptied state field on checkout submit resulting in 'Shipping/Billing State is a required field' errors
    </li>
  </ul>
  <p>
    <strong>Version 2.34.2 - 2019.08.29</strong>
  </p>
  <ul>
    <li>New: Added support for Braintree for WooCommerce: <a href="https://wordpress.org/plugins/woo-payment-gateway/">https://wordpress.org/plugins/woo-payment-gateway/</a>
    </li>
    <li>Improved: Add the ability to restrict address autocomplete to specific countries: <a href="https://www.checkoutwc.com/documentation/how-to-add-country-restrictions-to-address-autocomplete">https://www.checkoutwc.com/documentation/how-to-add-country-restrictions-to-address-autocomplete</a>
    </li>
    <li>Fix: Fix bug with Smart Send
    </li>
    <li>Fix: Fix edge case bug with WP Rocket CDN settings.
    </li>
    <li>Fix: Fix login is optional translation.
    </li>
    <li>Fix: Fix styling of cart subtotal to prevent line wrap.
    </li>
    <li>Fix: Removed Amazon Pay banner from Order Pay page.
    </li>
    <li>Fix: Fix bug with Braintree and PayPal for WooCommerce.
    </li>
    <li>Fix: Fix bug with Smart Coupons send to multiple recipients option.
    </li>
  </ul>
  <p>
    <strong>Version 2.34.1 - 2019.08.21</strong>
  </p>
  <ul>
    <li>Improved: Added cfw_show_logout_link filter to show the a log out link.
    </li>
    <li>Fix: Fixed issue where 'Return to cart' and 'Enter Promo Code' weren't translated.
    </li>
    <li>Fix: Fixed issue where WooCommerce German Marketplace added a fax field to the billing and shipping fields.&nbsp;
    </li>
    <li>Fix: Fixed issue where WooCommerce Checkout Field Editor was enforcing required states of billing / shipping address fields added prior to adding support to CheckoutWC.
    </li>
    <li>Fix: Fixed how select labels appear. They now appear at all times so that selects with empty placeholders are identifiable.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.34.0 - 2019.08.19</strong>
  </p>
  <ul>
    <li>ðŸŽ‰&nbsp;NEW: Support for WooCommerce Checkout Field Editor. Due to the custom nature of our forms, we can only support&nbsp;<strong>Additional Fields.&nbsp;</strong>When both plugins are active, we hide the Billing and Shipping tabs from the field editor screen.
    </li>
    <li>New: Added support for Listable theme.
    </li>
    <li>Improved: Upped WooCommerce supported version to 3.7.0.
    </li>
    <li>Improved: Square Recurring Payments fields are now styled better.
    </li>
    <li>Fixed: Fixed save card checkbox styles.
    </li>
    <li>Fixed: Fix issue where Indeed Affiliates Pro broke select styles.
    </li>
    <li>Fixed: Fixed issue where Verso theme loaded search widget at the bottom of the checkout page.
    </li>
    <li>Fixed: Added back support for Square 1.x
    </li>
  </ul>
  <p>
    <strong>Version 2.33.3 - 2019.08.09</strong>
  </p>
  <ul>
    <li>Improved: Added console logging for Ajax request errors during complete order calls.
    </li>
    <li>Fix: Fix bugs with state field requirement during country switches.
    </li>
    <li>Fix: Phone field validation now matches other fields.
    </li>
    <li>Fix: Filter out empty error messages during update checkout.
    </li>
    <li>Fix: Fix potential JS errors where Square is loaded but not available due to cart conditions.
    </li>
    <li>Fix: Don't run payment gateway form fields through cfw_form_field.
    </li>
    <li>Fix: Styling fixes for SkyVerge payment gateway fields.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.33.2 - 2019.08.06</strong>
  </p>
  <p>
    Minor patches for specific theme and plugin configurations. If you do not need them, you can wait to update if you prefer. All of these updates are minor and should not impact sites that do not use the affected themes or plugins.
  </p>
  <ul>
    <li>Fix: Patch for Verso theme.
    </li>
    <li>Fix: Patch for Optimizer theme.
    </li>
    <li>Fix: Patch for Strollik Core plugin.&nbsp;
    </li>
    <li>Fix: Add missing Checkout object to woocommerce_after_checkout_form hook. This is needed by Klaviyo, and probably other plugins.
    </li>
  </ul>
  <p>
    <strong>Version 2.33.1 - 2019.08.03</strong>
  </p>
  <ul>
    <li>Hotfix: Fix bug where stylesheet / JavaScript assets did not load unless dev mode flag was set to true.
    </li>
  </ul>
  <p>
    <strong>Version 2.33.0 - 2019.08.02</strong>
  </p>
  <ul>
    <li>New: Added support for Atik theme.
    </li>
    <li>Improved: Get rid of Dotenv library which is unnecessary and caused issues with users who had different versions of the same library loaded.
    </li>
    <li>Improved: Move handling of woocommerce_form_field so that transformations apply during update_checkout
    </li>
    <li>Fix: Fix issue with Square 2.0.&nbsp;
    </li>
    <li>Fix: Fix issues with Webshipper pickup points.
    </li>
    <li>Fix: Fix issue where unshipped carts calculated taxes incorrectly due to geolocation.&nbsp;
    </li>
    <li>Fix: Fix JS error when no payment methods are available.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.32.1 - 2019.07.24</strong>
  </p>
  <ul>
    <li>Improved: Added warning notice in admin dashboard about incompatible plugins.
    </li>
    <li>Improved: Added filter to highlight certain countries in list of countries above the rest of the list: cfw_highlighted_countries
    </li>
    <li>Improved: Added filter for enabling Elementor assets (stylesheet / javascript) on the checkout page: cfw_block_elementor_assets
    </li>
    <li>Improved: Added support for number fields.
    </li>
    <li>Improved: Corrected Square 2.0 credit card field styles.
    </li>
    <li>Improved: Updated translation files.
    </li>
    <li>Fix: Fix for Futurist breadcrumbs when header background color is white.
    </li>
    <li>Fix: Fix bug where active tab class was not present on initial page load.
    </li>
    <li>Fix: Fix bugs with Amazon Payments.
    </li>
  </ul>
  <p>
    <strong>Version 2.32.0 - 2019.07.23</strong>
  </p>
  <ul>
    <li>New: Support for Country Based Payments
    </li>
    <li>New: Beta support for German Marketplace
    </li>
    <li>Improved: Added cfw_return_to_cart_link_url and cfw_return_to_cart_link_text filters.
    </li>
    <li>Improved: Added billing and shipping level information to autocomplete attributes.
    </li>
    <li>Improved: Added cfw_login_optional_text filter.
    </li>
    <li>Fix: Fix filters for changing promo code field label.
    </li>
  </ul>
  <p>
    <strong>Version 2.31.2/2.31.3 - 2019.07.19</strong>
  </p>
  <ul>
    <li>Fix: Fix fatal error for sites running &lt; PHP 7.1. Implemented automatic compatibility scanning to prevent incompatible PHP code from being released in the future.
    </li>
    <li>Fix: Fix fatal error when loading customizer.
    </li>
    <li>Fix: Fix bug where shipping method list doesn't update when applying coupons.
    </li>
    <li>Fix: Fix bug where style overrides from Design tab didn't work in production builds.
    </li>
  </ul>
  <p>
    <strong>Version 2.31.1 - 2019.07.18</strong>
  </p>
  <ul>
    <li>Hotfix: Fix fatal error on Design tab in admin settings.
    </li>
  </ul>
  <p>
    <strong>Version 2.31.2 - 2019.07.19</strong>
  </p>
  <ul>
    <li>Fix: Fix fatal error for sites running &lt; PHP 7.1. Implemented automatic compatibility scanning to prevent incompatible PHP code from being released in the future.
    </li>
    <li>Fix: Fix fatal error when loading customizer.
    </li>
    <li>Fix: Fix bug where shipping method list doesn't update when applying coupons.
    </li>
  </ul>
  <p>
    <strong>Version 2.31.0 - 2019.07.18</strong>
  </p>
  <ul>
    <li>ðŸ¾ NEW: Added support for order-pay checkout endpoint. Disabled by default. <a href="https://www.checkoutwc.com/documentation/how-to-enable-order-pay-support">More information here.</a>
    </li>
    <li>Improved: Refactored template management and loading classes.
    </li>
    <li>Improved: Refactored zip autocomplete class.
    </li>
    <li>Improved: Added cfw_promo_code_label filter.
    </li>
    <li>Improved: Added active tab class to form.
    </li>
    <li>Improved: Consolidated how notices are output on the checkout page on first load.
    </li>
    <li>Fix: Fix issue where having exactly 10 items in your cart caused the quantity dropdown to show 'Delete'.
    </li>
  </ul>
  <p>
    <strong>Version 2.30.1 - 2019.07.17</strong>
  </p>
  <ul>
    <li>Fix: Fix bug that prevented shipping address preview from updating on shipping method tab.
    </li>
  </ul>
  <p>
    <strong>Version 2.30.0 - 2019.07.17</strong>
  </p>
  <p>
    This update includes some refactoring. We tested these changes extensively and with our automated testing tools, but we cannot test every configuration.&nbsp; <strong>Please make sure you test on a staging site before updating your live site.</strong>
  </p>
  <ul>
    <li>Improved: Refactored totals area to use more native structure (table) for better 3rd party plugin support.
    </li>
    <li>Improved: Cleaned up Update Checkout script to use fragment approach from native WooCommerce.
    </li>
    <li>Fix: Add missing woocommerce_checkout_before_order_review / woocommerce_checkout_after_order_review hooks to Copify and Futurist templates.
    </li>
    <li>Fix: Fix issue with Checkout Add-ons outputting their fields in the wrong place.
    </li>
    <li>Fix: Fix issue with extra total row when using MyCred Partial Payments.
    </li>
    <li>Fix: Fix issue with cart editing where dynamic discounts didn't calculate properly.
    </li>
    <li>Fix: Fix issue where having more than 10 units of a cart item conflicted with cart editing.
    </li>
    <li>Fix: Fix issue with Klaviyo where carts were not tracked properly.
    </li>
  </ul>
  <p>
    <strong>Version 2.29.1 - 2019.07.13</strong>
  </p>
  <ul>
    <li>Fix: Fix styling of Stripe radio buttons.
    </li>
    <li>Fix: Don't show tax line if WooCommerce is configured to show taxes inclusively in the cart / checkout.
    </li>
  </ul>
  <p>
    <strong>Version 2.29.0 - 2019.07.11</strong>
  </p>
  <ul>
    <li>New: Added support for MyCred Partial Points as well as other plugins that use woocommerce_checkout_before_order_review / woocommerce_checkout_after_order_review hooks.
    </li>
    <li>Fix: Fix issue with Zidane theme.
    </li>
    <li>Fix: Fix issue where includes were not being loaded correctly for one site.
    </li>
    <li>Fix: Fix issue with WooCommerce Germanized that prevented Klarna Payments from working properly.
    </li>
    <li>Fix: Fix issue where removing a WooCommerce Subscription product with cart editing left the recurring totals table.
    </li>
  </ul>
  <p>
    <strong>Version 2.28.0 - 2019.07.10</strong>
  </p>
  <ul>
    <li>Improved: Checkboxes and radio buttons now use the same styling that Shopify uses.
    </li>
    <li>Improved: All fields now have a slight transition, causing the field outline and check/uncheck to animate slightly.
    </li>
    <li>Improved: When using Address Autocomplete, Address Line 1 is formatted based on the country. So for applicable countries, the address will be formatted Main St 100, instead of the US format (100 Main St)
    </li>
    <li>Improved: Fonts are now rendered with subpixel antialiasing where supported for a smoother look and feel.
    </li>
  </ul>
  <p>
    <strong>Version 2.27.0 - 2019.07.09</strong>
  </p>
  <ul>
    <li>ðŸŽ‰ NEW: Address Autocomplete is here! Customers can now quickly and accurately locate their address using Google Maps.&nbsp;<strong>Requires a Growth or Agency license to enable.&nbsp;</strong><a href="https://www.checkoutwc.com/documentation/how-to-enable-address-autocomplete">More information.</a>
    </li>
    <li>Fix: Fixed issue where WooCommerce Extra Checkout Fields for Brazil removed the phone fields.&nbsp;
    </li>
    <li>Fix: Fixed issue where Order Notes field is not displayed properly.
    </li>
  </ul>
  <p>
    <strong>Version 2.26.1 - 2019.07.08</strong>
  </p>
  <ul>
    <li>New: Added support for Divi Ultimate Header / Footer.
    </li>
    <li>Improved: Added cfw_place_order_button_container_classes filter.
    </li>
    <li>Improved: You can now use shortcodes in footer text.
    </li>
    <li>Fix: Fixed bug with theme compatibility classes that prevented them from loading properly.
    </li>
    <li>Fix: Fixed issue where WooCommerce Germanized prevented order button from appearing.
    </li>
  </ul>
  <p>
    <strong>Version 2.26.0 - 07/04/2019</strong>
  </p>
  <p>
    Happy 4th to those of you hailing from the USA. This release has a pretty significant change regarding how fields from other plugins are rendered. As always, we recommend you test before deploying to a live site.
  </p>
  <ul>
    <li>New: Added filter to suppress empty cart notice after redirect when using Cart Editing: cfw_cart_edit_redirect_suppress_notice
    </li>
    <li>Improved: All calls to woocommerce_form_field are now rerouted through cfw_form_field for styling / UI consistency.&nbsp;
    </li>
    <li>Improved: Consolidate support for plugins that add UI after the shipping options. Adds support for Pakettikauppa.
    </li>
    <li>Fix: Fixed bug where Braintree PayPal buttons didn't load consistently
    </li>
    <li>Fix: Added a workaround for a glitch with CO2OK and our tab system until they can fix this: <a href="https://github.com/Mil0dV/co2ok-plugin-woocommerce/issues/32">https://github.com/Mil0dV/co2ok-plugin-woocommerce/issues/32</a>
    </li>
  </ul>
  <p>
    <strong>Version 2.25.0 - 07/01/2019</strong>
  </p>
  <ul>
    <li>New: Added option to set the URL that checkout redirects to if the cart is emptied during cart editing.
    </li>
    <li>New: Added translations for Finland!
    </li>
    <li>New: SendCloud support!
    </li>
    <li>Improved: Added protection to prevent JS errors with Braintree.
    </li>
    <li>Improved: Hidden fields no longer get wrap containers.
    </li>
    <li>Improved: When advancing from customer information tab, all fields that have errors now highlight at the same time.
    </li>
    <li>Improved: Portuguese field validation messages now load correctly.
    </li>
    <li>Improved: Cleaned up some undefined index notices.
    </li>
    <li>Fix: Removed WOOCOMMERCE_CART constant that was causing some issues during coupon application.
    </li>
    <li>Fix: Removed redundant cart totaling call during apply coupon action.
    </li>
    <li>Fix: Fixed Klarna Payments
    </li>
    <li>Fix: Fixed several bugs with NL Postcode Checker.
    </li>
    <li>Fix: Fixed several bugs with PostNL.
    </li>
    <li>Fix: Missing field validation translation files no longer throws a JS error.
    </li>
  </ul>
  <p>
    <strong>Version 2.24.1 - 06/26/2019</strong>
  </p>
  <p>
    Sorry for the double release. We didn't see this bug until 2.24.0 was out the door, but fortunately this was a simple fix.&nbsp;
  </p>
  <ul>
    <li>Hotfix: Fix bug where billing address overwrites shipping address.
    </li>
  </ul>
  <p>
    <strong>Version 2.24.0 - 06/26/2019</strong>
  </p>
  <ul>
    <li>ðŸŽ‰ NEW: Cart editing is here! Customers can now adjust the quantity or remove cart items from checkout.&nbsp;<strong>Requires a Growth or Agency license to enable.&nbsp;</strong><a href="https://www.checkoutwc.com/documentation/how-to-enable-cart-editing">More information.</a>
    </li>
    <li>Improved: Account exists AJAX call is now throttled to prevent waste of server resources.
    </li>
    <li>Fixed: Field validation messages now works with Norwegian translations.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.23.2 - 06/26/2019</strong>
  </p>
  <ul>
    <li>Emergency Hotfix: Fix bug in 2.23.1 that allowed theme stylesheets, etc to leak into checkout page.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.23.1 - 06/25/2019</strong>
  </p>
  <ul>
    <li>Improved: Improved Norwegian translations. Hat tip: Martin O.
    </li>
    <li>Fixed: Fixed issue where empty coupon message caused errors that break checkout.
    </li>
    <li>Fixed: Fixed issue where The7 theme compatibility fixes were applying on normal pages. This involved a slight refactor of the compatibility classes to prevent this from happening with other compatibility classes.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.23.0 - 06/21/2019</strong>
  </p>
  <ul>
    <li>New: Added&nbsp;<strong>Cart Summary Mobile Label</strong>&nbsp;setting to make it easier to override the mobile cart link label. <a href="https://www.checkoutwc.com/documentation/how-to-change-show-order-summary-text-on-mobile-cart">More information.</a>
    </li>
    <li>Improved: Added preliminary support for WooCommerce Address Validation with SmartyStreets. Implementation has some glitches, but this is a start.
    </li>
    <li>Improved: Added shim for default ship_to_different_address field. Before we were using this field to essentially mean the opposite of what it means on the default checkout because our address order is reversed. Now we have added an invisible shim for plugins that check this value that has a predictable, normal value and added a separate field for handling showing/hiding the billing address.&nbsp;
    </li>
    <li>Improved: Added cfw_cart_html filter to allow filtering the cart html.
    </li>
    <li>Fix: Added js-cookie to main script dependencies because some plugins expect this.
    </li>
    <li>Fix: Fixed issue with The7 theme styles leaking into checkout page.
    </li>
    <li>Fix: Fixed issue with Elementor styles messing up the checkout page.
    </li>
    <li>Fix: Fixed issue with WP admin bar display position on mobile.
    </li>
  </ul>
  <p>
    <strong>Version 2.22.0 - 06/12/2019</strong>
  </p>
  <ul>
    <li>New: Added a Recommended Plugins tab to highlight plugins that work well with CheckoutWC.
    </li>
    <li>New: Added Polish translation files.
    </li>
    <li>Improved: Mondial Relay now prevents advancing to payment method tab if pickup point is not selected.
    </li>
    <li>Improved: License key is now a password field to prevent other users from copying it (as easily)
    </li>
    <li>Improved: Refactored billing and payment radio groups to get rid of extra div wrapper.
    </li>
    <li>Improved: Phone field is now handled through native WooCommerce customizer setting. Previous CheckoutWC setting is migrated to WooCommerce setting on update.&nbsp;
    </li>
    <li>Fixed: Added Slovenian Parsley translations.
    </li>
    <li>Fixed: Removed PHP notice.
    </li>
    <li>Fixed: Added missing callbacks to WooCommerce action calls.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.21.1 - 06/04/2019</strong>
  </p>
  <ul>
    <li>New: Added Square Recurring / Simple Payments For WooCommerce Subscriptions support.
    </li>
    <li>New: Added Danish translations.
    </li>
  </ul>
  <p>
    <strong>Version 2.21.0 - 06/02/2019</strong>
  </p>
  <ul>
    <li>New: Added support for Jupiter theme.
    </li>
    <li>New: Added cfw_show_cart_item_discount filter to show discount of cart items.
    </li>
    <li>New: Added support for SUMO Payment Plans.
    </li>
    <li>Improved: Added cfw_mondial_link_location filter to control Mondial Relay chooser location.
    </li>
    <li>Fixed: Fixed issue where state fields would reset when clicking Complete Order button.
    </li>
    <li>Fixed: Fixed bug where selecting a country that doesn't support the city field after setting the country to a country with city fields prevented advancing to the shipping method tab.
    </li>
  </ul>
  <p>
    <strong>Version 2.20.4 - 05/22/2019</strong>
  </p>
  <ul>
    <li>New: Added cfw_force_display_billing_address which allows you to force the billing address fields to always show. (Removes the "Same as shipping address" option)
    </li>
    <li>New: Added Slovenian and Norwegian translations.&nbsp;
    </li>
    <li>Improved: Using cfw_form_field to output more fields so they show up with our styling.
    </li>
    <li>Fix: When shipping tab hidden, previous tab label had wrong tab name.
    </li>
    <li>Fix: When shipping tab hidden, validation of billing fields was sometimes incorrect.&nbsp;
    </li>
    <li>Fix: Fixed issue with URL used for license activation / deactivation. If you see any problems, reactivating your license should fix any issues.
    </li>
  </ul>
  <p>
    <strong>Version 2.20.3 - 05/15/2019</strong>
  </p>
  <ul>
    <li>Fix: Fixed bug that caused infinite loop when WooCommerce Subscriptions is set to not allow mixed carts.&nbsp;
    </li>
    <li>Improved: The fix above greatly simplifies how we identify and suppress add to cart notices when add to cart action redirects to checkout. Win win win.
    </li>
  </ul>
  <p>
    <strong>Version 2.20.2 - 05/14/2019</strong>
  </p>
  <ul>
    <li>Improved: Pass data to update_checkout that WooCommerce passes.
    </li>
    <li>Fix: Fixed Klarna Checkout integration
    </li>
    <li>Fix: Fixed Martfury theme compatibility.
    </li>
    <li>Fix: Fixed a few glitches with Mondial Relay.&nbsp;
    </li>
    <li>Fix: Fixed compatibility with WPML language switcher on checkout page.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.20.1 - 05/10/2019</strong>
  </p>
  <ul>
    <li>Improved: We found a better way to be compatible with plugins that expect the WooCommerce scripts to be loaded, allowing us to simplify a few of our compatibility classes and remove one.&nbsp;
    </li>
    <li>Improved: Include CSS that prevents Mondial Relay from hiding the shipping address fields.
    </li>
    <li>Fix: Fixed bug where Braintree fields reset when editing billing fields.
    </li>
    <li>Fix: Fixed an edge case bug with calculating form field rows.
    </li>
  </ul>
  <p>
    <strong>Version 2.20.0 - 05/08/2019</strong>
  </p>
  <p>
    âš&nbsp;ï¸ If you had a problem with your license deactivating itself randomly, we are really sorry. It only affected a small number of customers, but that's no excuse!
  </p>
  <p>
    This release has a permanent fix, but&nbsp; <strong>after you update</strong>please go to Settings &gt; Checkout for WooCommerce &gt; License and click "Deactivate" and then "Activate" again. This will ensure you have no future problems!
  </p>
  <ul>
    <li>Fix: Fixed issues with PostNL
    </li>
    <li>Fix: Fixed issues with WC Postcode Checker.
    </li>
    <li>Fix: Fixed bug with EU VAT Number not removing VAT as expected.
    </li>
    <li>Fix: Fixed issues with Mondial Relay shipping provider.
    </li>
    <li>Fix: Fixed issue where cart summary background color was not respected on mobile.
    </li>
    <li>Fix: Fixed issue with inconsistent licensing URL for activations. Also ensure customers using WPML will not have issues with their license remaining active.
    </li>
  </ul>
  <p>
    <strong>Version 2.19.1 - 05/07/2019</strong>
  </p>
  <ul>
    <li>Fix: Fixed bug where 3rd party plugins calling update checkout threw a JS error.
    </li>
  </ul>
  <p>
    <strong>Version 2.19.0 - 05/07/2019</strong>
  </p>
  <p>
    This release continues to refactor the JS that runs the checkout page to make it simpler, more robust, and easier to debug. We test extensively with automated and manual tests, but as always please test before updating your live site. Your site is different than our test sites!
  </p>
  <ul>
    <li>New: Added support for Mondial Relay shipment provider.
    </li>
    <li>Improved: Added 3 coupon related JavaScript events: cfw-apply-coupon-success, cfw-apply-coupon-failure, cfw-apply-coupon-error,&nbsp;cfw-apply-coupon-complete
    </li>
    <li>Improved: Added UI blocking to dynamic areas of the checkout page. During updates, the shipping address preview, shipping methods, cart, and place order button fade out and are unclickable until the checkout is up to date.&nbsp;
    </li>
    <li>Improved: When a update_checkout call errors out because the server times out, or any other reason, the blocked UI portions will unblock. This ensures users can always retry without refreshing the page.
    </li>
    <li>Improved: Ensure all update_checkout calls use queueing system.
    </li>
    <li>Improved: Applying coupons doesn't send the shipping method. This matches core and allows for changing the selected shipping method when a coupon is applied.
    </li>
    <li>Fix: Fixed critical bug where validation script blocked checkout submit for some users.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.18.2 - 05/03/2019</strong>
  </p>
  <ul>
    <li>Fix: Added compatibility for Atelier theme.
    </li>
  </ul>
  <p>
    <strong>Version 2.18.1 - 05/03/2019</strong>
  </p>
  <ul>
    <li>FIX: Fixed fatal error on some configurations resulting in checkout page that does not load.
    </li>
    <li>Improved: Added filter to override which URL is used for licensing checks.
    </li>
  </ul>
  <p>
    <strong>Version 2.18.0 - 05/02/2019</strong>
  </p>
  <p>
    This release contains some changes to field labels and placeholders. All optional fields now include "(optional)" at the end of the placeholder and label. This is in keeping with best practices.&nbsp;Also, we're using the native WooCommerce label for address_2, so instead of the abbreviation "Apt" it's now spelled out "Apartment".&nbsp;
  </p>
  <p>
    Lastly, the address_2 field is now full width. This mitigates some display issues on smaller screens where the label was cut off. You can always remove this field entirely by <a href="https://www.checkoutwc.com/documentation/how-to-remove-address-line-2">following this guide.</a>
  </p>
  <ul>
    <li>Improved: Consistently apply optional notice to all optional fields.
    </li>
    <li>Use WooCommerce native translation for most address fields.
    </li>
    <li>Fix IE11 bug that showed select dropdown for countries without states.
    </li>
    <li>Further improve cfw_form_field function automaticity.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.17.2 - 04/30/2019</strong>
  </p>
  <ul>
    <li>Fix: Fixed add to cart notice suppression when redirecting to checkout with WooCommerce Direct Checkout or conventional methods.
    </li>
    <li>Also: Updated WooCommerce tested version number.
    </li>
  </ul>
  <p>
    <strong>Version 2.17.1 - 04/29/2019</strong>
  </p>
  <ul>
    <li>Oops! We left out a fix for form persistence with the state field and a label formatting fix for the Address Line 2.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.17.0 - 04/29/2019</strong>
  </p>
  <p>
    Another release, another round of refactoring. As always, please test before deploying to your live site. We test fanatically, but we can't test every configuration.
  </p>
  <ul>
    <li>Improved: We're using vanilla WooCommerce localization scripts now. This sounds minor, but it was actually a pretty big refactor that fortunately allowed us to remove a lot of code that was proving to be difficult to maintain.
    </li>
    <li>Improved: Improved styling of recurring totals and before totals areas of cart summary.&nbsp;
    </li>
    <li>Fixed: Fixed a few Firefox styling issues related to field heights and credit card icons.
    </li>
  </ul>
  <p>
    <strong>Version 2.16.1 - 04/26/2019</strong>
  </p>
  <p>
    ðŸš¨IMPORTANT: This update includes an important fix that requires a small template change. Please follow this guide to update your template after updating to 2.16.1.
  </p>
  <ul>
    <li>Fix: WooCommerce 3.6 made a change to how customer data is loaded on the checkout page. Our attempts to fix this in 2.16.0 caused an issue with validation that caused a small number of stores to fail checkout submission for a fresh session in an incognito window. This is fixed now and we're very sorry for any disruptions this may have caused.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.16.0 - 04/24/2019</strong>
  </p>
  <p>
    This update has quite a few fixes in it. As always, please test before deploying to your live site. ðŸ™
  </p>
  <ul>
    <li>Add additional check to PayPal Checkout button to try to prevent double place order buttons.
    </li>
    <li>Automatic field row calculations and wraps which allows us to simplify our field API.
    </li>
    <li>Added default error when payment gateway doesn't return a reason for failure.
    </li>
    <li>Added framework for add-on settings. (Coming soon!)
    </li>
    <li>Added some additional action hooks to templates.
    </li>
    <li>Fixed German translation of phone field setting in admin.
    </li>
    <li>Fixed JS errors caused by PostNL.
    </li>
    <li>Fixed but with Martfury theme add-on plugin.
    </li>
    <li>Fixed bug with Stripe gateway Apple Pay / Google Pay buttons showing two OR dividers.
    </li>
    <li>Fixed bug where state dropdown did not repopulate correctly on refresh.
    </li>
    <li>Fixed bug with Pakkelabels modal not showing up.
    </li>
    <li>Fixed bug where selecting a shipping method caused an extra update_checkout call.
    </li>
    <li>Prevent WC Fields Factory from messing up checkout fields.
    </li>
    <li>Added logout link for Amazon Pay and fixed layout / widget placement bugs.
    </li>
    <li>Removed some PHP notices.
    </li>
  </ul>
  <p>
    <strong>Version 2.15.2 - 04/14/2019</strong>
  </p>
  <ul>
    <li>Fixed: Braintree's hosted fields&nbsp;<em>really</em>don't want to load if they are not visible. To fix this, we have added a one time event that refreshes the Braintree fields after the payment tab loads. This fixes all of the issues we have been having with the fields not loading correctly.
    </li>
  </ul>
  <p>
    <strong>Version 2.15.1 - 04/13/2019</strong>
  </p>
  <p>
    Sometimes when your children keep you awake half of the night, you end up refactoring code in your head. My insomnia is your reward. ðŸ˜´
  </p>
  <ul>
    <li>Fix: Refactored the fix for PayPal for WooCommerce billing field validation errors to be simpler and more robust. Now works for logged in users and logged out users.
    </li>
  </ul>
  <p>
    <strong>Version 2.15.0 - 04/12/2019</strong>
  </p>
  <ul>
    <li>Fix: Fixed bug where billing states did not load correctly.
    </li>
    <li>Fix: Fixed bug where PayPal for WooCommerce was unable to validate billing fields during express checkout.
    </li>
    <li>Fix: Fixed bug where Braintree credit card fields do not load.
    </li>
  </ul>
  <p>
    <strong>Version 2.14.0 - 04/11/2019</strong>
  </p>
  <p>
    This release does some minor refactoring to help broaden compatibility with other plugins. We re-tested a number of common plugins, but there's always a chance there will be an unintended side effect.&nbsp; <strong>Please test yourself before updating! (Which you should always do anyway ðŸ˜ƒ)</strong>
  </p>
  <ul>
    <li>Improved: Fixed bug with WooCommerce 3.6-rc2
    </li>
    <li>Improved: State label will now use the localized version such as "Region"
    </li>
    <li>Improved: State select now renders with floating label at all times, not just when you select a state.
    </li>
    <li>Improved: Added support for woocommerce_checkout_before|after_customer_details hooks from WooCommerce core.
    </li>
    <li>Improved: Added more compatibility for adding fields with woocommerce_checkout_fields filter.
    </li>
  </ul>
  <p>
    <strong>Version 2.13.9 - 04/09/2019</strong>
  </p>
  <ul>
    <li>Added support for WooFunnels Order Bumps.
    </li>
  </ul>
  <p>
    <strong>Version 2.13.8 - 04/05/2019</strong>
  </p>
  <ul>
    <li>New: Added support for YITH Gift Cards Premium.
    </li>
    <li>Fix: Fixed bug where Square fields don't load if it's the only gateway.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.13.7 - 04/03/2019</strong>
  </p>
  <ul>
    <li>Improved: Move dev dependencies into require-dev and remove from release builds. Build size improved by 15%!
    </li>
    <li>Improved: Added cfw_create_account_site_name filter to modify site name in "Create % shopping account" text.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.13.6 - 04/02/2019</strong>
  </p>
  <ul>
    <li>Hotfix: Fix translation of "Show order summary". Sorry about that!
    </li>
  </ul>
  <p>
    <strong>Version 2.13.5 - 04/01/2019</strong>
  </p>
  <ul>
    <li>New: Support for BlueCheck!
    </li>
    <li>Improved: Added cfw_show_order_summary_link_text filter to allow "Show order summary" text to be overridden.&nbsp;
    </li>
    <li>Improved: Added more space for cart item prices on mobile.&nbsp;
    </li>
    <li>Fix: Fixed translation with NL Postcode Checker for "Street name" placeholder.&nbsp;
    </li>
    <li>Fix: Fixed bug where subscriptions with free trials weren't purchasable because payment fields didn't render.&nbsp;
    </li>
    <li>Fix: Fixed bug with Astra pro add-on.&nbsp;
    </li>
    <li>Fix: Fixed bug where applying 100% coupon (or otherwise making a paid order free) didn't update payment methods.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.13.4 - 03/29/2019</strong>
  </p>
  <ul>
    <li>New: Support for Order Delivery Date
    </li>
    <li>Improved: Removed some unnecessary nonce checks.&nbsp;
    </li>
    <li>Fix: Fixed bug with running CheckoutWC inside a subfolder install.&nbsp;
    </li>
    <li>Fix: Fixed bug with NL Postcode Checker not sending an address_1 field.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.13.3 - 03/27/2019</strong>
  </p>
  <ul>
    <li>Fix: Fixed bug with Avada theme.
    </li>
    <li>Fix: Fixed bug with OceanWP theme and OceanWP add-ons.
    </li>
    <li>Fix: Fixed localization bug with NL Postcode Checker.
    </li>
    <li>Fix: Street name and house number now render correctly when using NL Postcode Checker or PostNL.
    </li>
  </ul>
  <p>
    <strong>Version 2.13.2 - 03/26/2019</strong>
  </p>
  <ul>
    <li>Hotfix: Fatal error that prevents summary area from loading when PayPal for WooCommerce is enabled.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.13.1 - 03/25/2019</strong>
  </p>
  <ul>
    <li>New: Support for Savoy theme
    </li>
    <li>Improved: PostNL and NL Postcode Checker fields now render correctly without duplicated / extra fields.&nbsp;
    </li>
    <li>Fix: 2.13.0 added support for a WooCommerce hook that was apparently used by a number of gateways to add notices we don't want on the checkout page. We've cleaned these up on a case by case basis and the problems should be fixed.
    </li>
    <li>Fix: Fixed styling of woocommerce-error divs that were not inside our alert container.
    </li>
  </ul>
  <p>
    <strong>Version 2.13.0 - 03/23/2019</strong>
  </p>
  <ul>
    <li>New: Support for Smart Offers, Checkout Countdown Timer, and any plugin that uses woocommerce_before_checkout_form
    </li>
    <li>Improved: Optimized autoloader and removed an unused PHP library
    </li>
    <li>Improved: Removed a number of compatibility classes that are no longer required. Parity FTW.âœŒðŸ»
    </li>
    <li>Fixed: Fixed bug with Square gateway where fields wouldn't render if they were not visible on page load.
    </li>
  </ul>
  <p>
    <strong>Version 2.12.0 - 03/20/2019</strong>
  </p>
  <ul>
    <li>New: YITH Points and Rewards support
    </li>
    <li>Fix: Bug with Astra theme
    </li>
    <li>Fix: Bug with PostNL 3.x
    </li>
  </ul>
  <p>
    <strong>Version 2.11.3 - 03/19/2019</strong>
  </p>
  <ul>
    <li>Improved: We now detect server errors during checkout submit, login, coupon applications, etc allowing users to have more information about what is going on with their order.
    </li>
    <li>Fix: Fixed bug preventing address line 2 label overrides from working properly.
    </li>
    <li>House keeping: Removed some vestigial logging.ðŸ§¹
    </li>
  </ul>
  <p>
    <strong>Version 2.11.2 - 03/18/2019</strong>
  </p>
  <ul>
    <li>Improved: EU VAT Number now shows and hides based on the shipping country and whether or not "Same as shipping address" is checked.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.11.1 - 03/18/2019</strong>
  </p>
  <ul>
    <li>Hotfix: Fix an issue where EU VAT Number's field was displaying twice.
    </li>
  </ul>
  <p>
    <strong>Version 2.11.0 - 03/15/2019</strong>
  </p>
  <ul>
    <li>New: Support for Smart Send
    </li>
    <li>New: Full support for Webshipper. Drop points now display underneath shipping options.
    </li>
    <li>Improved: We added a queuing system similar to WooCommerce native for update_checkout calls. This should help slightly with performance as well as prevent tons of concurrent events.
    </li>
    <li>Improved: When PayPal Checkout is started from the cart (or product page) it will now fallback to the normal checkout page summary where the customer can simply click "Place order". We want to handle this within our template eventually, but due to complications this was the fastest path to success.
    </li>
    <li>Fixed: Fixed an edge case where one customer had a fatal error.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.10.2 - 03/04/2019</strong>
  </p>
  <ul>
    <li>Improved: Added support for woocommerce_cart_item_name filter.
    </li>
    <li>Improved: More consistently apply cfw_checkout_before|after_billing|shipping_address actions.
    </li>
    <li>Improved: Add support for woocommerce_before_checkout_billing_form, woocommerce_after_checkout_billing_form, woocommerce_before_checkout_shipping_form, woocommerce_after_checkout_shipping_form actions.
    </li>
    <li>Improved: Validate phone fields like we do other fields.&nbsp;
    </li>
    <li>Fixed: Bug with free orders and Stripe gateway. (Improved how we transition to free order state)
    </li>
  </ul>
  <p>
    <strong>Version 2.10.1</strong>
  </p>
  <ul>
    <li>New: Added Hungarian language translation!
    </li>
    <li>Improved: Consolidated our is_checkout check into a single function.&nbsp;
    </li>
    <li>Fixed: Bug with GeneratePress theme styles on thank you page.
    </li>
    <li>Fixed: TM Organik theme includes some JS that fails on the checkout page. We worked around it.
    </li>
    <li>Fixed: Beaver Builder theme was loading some styles from its cache that affected the checkout page. It can't now!
    </li>
  </ul>
  <p>
    <strong>Version 2.10.0</strong>
  </p>
  <ul>
    <li>New: Add opt-in anonymous stat collection. Help us make CheckoutWC better!
    </li>
    <li>New: Support for YITH Deals Premium
    </li>
    <li>New: Add support for Pakkelabels
    </li>
    <li>New: Added&nbsp;cfw_check_create_account_by_default filter so that you can set the default checked state of the create account checkbox. More information here: <a href="https://www.checkoutwc.com/documentation/how-to-set-create-account-checkbox-to-unchecked-by-default">https://www.checkoutwc.com/documentation/how-to-set-create-account-checkbox-to-unchecked-by-default</a>
    </li>
    <li>New: Added support for Facebook for WooCommerce
    </li>
    <li>Improved: Detect PHP versions before 5.6 to prevent fatal error. (Plugin will activate, but not do anything - we will add a notice in a future version)
    </li>
    <li>Improved: Cleaned up translation files to remove external translation domain strings.&nbsp;
    </li>
    <li>Improved: It only affects us but we managed to reduce our production build process from 5 minutes to 20 seconds. And that makes us happy.
    </li>
    <li>Fix: Fixed issue with Avada theme and order received page styling.
    </li>
    <li>Fix: Shipping Phone will now show up in admin again. Also, it will continue to show up even if the phone fields are subsequently disabled.
    </li>
    <li>Fix: Prevent jQuery Touch and other libraries from messing up the mobile cart open / close functionality.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.9.0</strong>
  </p>
  <ul>
    <li>New: Cart is now dynamically updated to support plugins like&nbsp;WooCommerce Price Based on Country.
    </li>
    <li>New: Added support for&nbsp;WooCommerce Price Based on Country.
    </li>
    <li>Fix: Prevent some WooCommerce scripts from loading at checkout that break things.
    </li>
    <li>Fix: Fixed bug with NL Postcode Checker where street address was not saved to the order.
    </li>
  </ul>
  <p>
    <strong>Version 2.8.2</strong>
  </p>
  <ul>
    <li>Fix bug with WooCommerce Germanized preventing PayPal Checkout from loading.
    </li>
  </ul>
  <p>
    <strong>Version 2.8.1</strong>
  </p>
  <ul>
    <li>Fix: Added back support for&nbsp;cfw_enable_zip_autocomplete filter.&nbsp;
    </li>
    <li>Fix: Remove left over console.log
    </li>
    <li>Improved: Better handle payment gateway inits after update_checkout called to prevent order of operations problems.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.8.0</strong>
  </p>
  <p>
    This release includes a big change to the template form tag wrap. It&nbsp; <em>shouldn't</em>effect custom templates, but if you are running a custom template (and even if you aren't)&nbsp;<strong>please test before updating a live site.</strong>
  </p>
  <ul>
    <li>Fix: Works properly with "WooCommerce Ajax add to cart" (https://wordpress.org/plugins/woo-ajax-add-to-cart/)
    </li>
    <li>Fix: PayPal buttons now load properly on the first page load on a new session.&nbsp;<em>PayPal buttons should seriously work all the time in every situation now.</em>If you had asked me as a child how much of my life I expected to be consumed with figuring out why PayPal buttons don't appear, I would have cried and said "What is a PayPal button?"
    </li>
    <li>Improved: Moved form wraps so that they wrap the entire checkout page. This is necessary to allow moving the checkout button to the sidebar. More information: <a href="https://www.checkoutwc.com/documentation/how-to-move-the-complete-order-button-to-the-cart-summary-sidebar">https://www.checkoutwc.com/documentation/how-to-move-the-complete-order-button-to-the-cart-summary-sidebar</a>
    </li>
  </ul>
  <p>
    <strong>Version 2.7.4</strong>
  </p>
  <ul>
    <li>New: Now supports gateways that dynamically update the complete order button text.&nbsp;
    </li>
    <li>Improved: We moved the checkout nonce field into the dynamically updated order button area. This will ensure that dynamically updated nonces get processed correctly.
    </li>
    <li>Improved: We now proactively suppress PHP warnings and notices on the checkout page, for those who have improperly configured servers.&nbsp;
    </li>
    <li>Improved: It hasn't come up, but we decided to proactively set cache discouraging HTTP headers on the checkout page.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.7.3</strong>
  </p>
  <ul>
    <li>Fix PHP warning.&nbsp;
    </li>
    <li>Fix bug with WooCommerce Germanized where the complete order button was not rendered.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.7.2</strong>
  </p>
  <ul>
    <li>Added a fallback method for rendering PayPal buttons. I didn't realize how much of my life would be spent asking myself the metaphysical nature of a PayPal button.&nbsp;
    </li>
    <li>Fix an issue where the shipping address preview didn't update on the shipping method tab.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.7.0/2.7.1</strong>
  </p>
  <p>
    You know that episode of Breaking Bad where Walt spends an hour hunting down a fly. That's 2.7.0 and we killed the fly. We killed it good.
  </p>
  <p>
    There were 51 commits in this release. Please review the change log before updating, and as always&nbsp; <strong>please test thoroughly before updating a live site.&nbsp;</strong>
  </p>
  <p>
    <img src="https://www.checkoutwc.com/wp-content/uploads/edd/2019/02/giphy.gif" alt="" width="398" height="230" />&nbsp;
  </p>
  <ul>
    <li>New: Added support for WP Gens Refer a Friend plugin.
    </li>
    <li>New: Added preliminary support for Checkout Add-ons 2.0 (not released, keep your shirt on!)
    </li>
    <li>New: Added support for WooCommerce Social Logins (Official extension from SkyVerge)
    </li>
    <li>New: Variations that do not show up in product titles now appear in a small table underneath cart items.
    </li>
    <li>New: We now fingerprint the payment gateway markup so we can detect if a checkout update changes it. This allows us to preserve credit card fields even when the price changes.&nbsp;
    </li>
    <li>Improved: And because of that, we can move the billing address and checkout add-ons to the bottom of the payment tab where they naturally belong!
    </li>
    <li>Improved: Added polyfill to fix a few IE11 issues.
    </li>
    <li>Improved: Cleaned up a lot of old code from 1.x for specific gateways. We don't need it and we don't want it!
    </li>
    <li>Improved: Simplified checkout updating behaviors to reduce the number of AJAX calls. Less server load and faster UI for the win!
    </li>
    <li>Improved: Refactored zip autocomplete to run separately from validation behaviors.&nbsp;
    </li>
    <li>Fixed: PayPal for WooCommerce and PayPal Checkout now display their buttons properly every time!
    </li>
  </ul>
  <p>
    <strong>Version 2.6.0</strong>
  </p>
  <p>
    In 2.6.0, we continue to squash bugs and add customer requested features. Thanks for helping make CheckoutWC better.&nbsp;ðŸ‘ðŸ¼
  </p>
  <ul>
    <li>Fixed: CheckoutWC JS and CSS were loading on the order received and order pay pages. Now they aren't.&nbsp;
    </li>
    <li>Fixed: Payment Request Button separator wasn't loading for PayPal for WooCommerce. Now it does!
    </li>
    <li>Fixed: Sometimes the wrong PayPal button would load on checkout when using PayPal for WooCommerce. Now the right one always loads.&nbsp;
    </li>
    <li>Fixed: When not using smart payment buttons with PayPal Checkout, the complete order button didn't appear. Now it does!
    </li>
    <li>Fixed markup error in templates that was not causing any bugs, but was bad and now it's been banished.&nbsp;
    </li>
    <li>Enhancement: We added 4 new action hooks:&nbsp;cfw_before_footer, cfw_after_footer,&nbsp;cfw_after_cart_summary_totals,&nbsp;cfw_after_cart_summary
    </li>
    <li>New: We now support EU VAT Number add-on from WooCommerce.&nbsp;
    </li>
    <li>New: We now support WooCommerce - Gift Cards (WP-Ronin)
    </li>
    <li>New: We now support Braintree from PayPal for WooCommerce!
    </li>
  </ul>
  <p>
    <strong>Version 2.5.3</strong>
  </p>
  <p>
    NOTE: If this is the first time you are upgrading from 2.4.x, please see the theme template note from release 2.5.0 below.
  </p>
  <ul>
    <li>Fix bug that prevented coupons from being applied.
    </li>
    <li>Fix how we handle jQuery as a dependency with web pack to prevent double loading jQuery.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.5.0/2.5.1/2.5.2</strong>
  </p>
  <p>
    âš&nbsp;ï¸ WARNING: If you are using a custom template, please read this BEFORE upgrading.&nbsp;âš&nbsp;ï¸
  </p>
  <ul>
    <li>Remove tests from release build to reduce size.
    </li>
    <li>Suppress add to cart notice on checkout page at all times.
    </li>
    <li>Refactor inline scripts to use wp_localize_script(). This should help shore up some compatibility problems with minification plugins. (Though YMMV)
    </li>
    <li>Fix bug with how billing address was handled during checkout submit.&nbsp;
    </li>
    <li>Fix bug with PayPal Checkout and an empty billing address at submit.
    </li>
    <li>Add support for WooCommerce Smart Coupons.
    </li>
    <li>2.5.1: Added support for WooCommerce PostNL
    </li>
    <li>2.5.1: Force jquery-migrate to load on checkout since some themes and plugins disable it.
    </li>
    <li>2.5.2: Fix issue with PayPal Checkout button not showing up properly.
    </li>
  </ul>
  <p>
    <strong>Version 2.4.16</strong>
  </p>
  <ul>
    <li>Enhancement: Add support for PayPal for WooCommerce 1.5.7 (preserves legacy support for now) (Hat tip: PayPal for WooCommerce team)
    </li>
    <li>Enhancement: When switching tabs, browser will scroll to the top of the container. This is especially helpful on mobile. (Hat tip: Rafael)
    </li>
    <li>Feature: Add cursory support for Ultimate Points and Rewards. (Hat tip: Chit)
    </li>
    <li>Feature: Add support for GeneratePress Premium. (Hat tip: Chit)
    </li>
    <li>Fix: Removed PHP warning in NL Postcode Checker compatibility class. (Hat tip: Hendrik)
    </li>
    <li>Fix: Fixed issue with plugin details inheriting CFW styles in a way that broke the rendering of the native modal.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.4.15</strong>
  </p>
  <ul>
    <li>Add support for ActiveCampaign for WooCommerce.
    </li>
  </ul>
  <p>
    <strong>Version 2.4.14</strong>
  </p>
  <ul>
    <li>Add form-row to a more logical place in the markup and use filters to move it for NL Postcode Checker.
    </li>
    <li>Add compatibility class for Porto theme to prevent it from loading stylesheets on the checkout page.&nbsp;
    </li>
    <li>Fix PHP syntax error in Direct Checkout compatibility class that caused issues &lt; PHP 7.x
    </li>
  </ul>
  <p>
    <strong>Version 2.4.13</strong>
  </p>
  <ul>
    <li>Add support for NL Postcode Checker.
    </li>
    <li>Add support for WooCommerce Direct Checkout.
    </li>
    <li>Fix&nbsp;AfterPay by Krokedil gateway.
    </li>
    <li>Improve MailChimp for WooCommerce support.
    </li>
    <li>Fix some Klarna Checkout styles.
    </li>
  </ul>
  <p>
    <strong>Version 2.4.12</strong>
  </p>
  <ul>
    <li>Fix faulty evaluation that caused a fatal error for some PayPal for WooCommerce configurations.
    </li>
  </ul>
  <p>
    <strong>Version 2.4.11</strong>
  </p>
  <ul>
    <li>Fix Klarna Checkout integration with support for fragment refresh system. Selecting Klarna from the list now performs the same action as clicking "Pay with Klarna" button.
    </li>
  </ul>
  <p>
    <strong>Version 2.4.10</strong>
  </p>
  <ul>
    <li>Add missing translation for Your Cart in Futurist theme.
    </li>
    <li>Fix bug where network activated WooCommerce was not properly detected.&nbsp;
    </li>
    <li>Fix field validation language library for Denmark.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.4.9</strong>
  </p>
  <ul>
    <li>Hotfix: Removed "Unknown error" alert that was showing up briefly during successful orders for some payment gateways.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.4.8</strong>
  </p>
  <ul>
    <li>Fix a bug that prevented Authorize.net (and possibly other gateways) from submitting properly. This was caused by our implementation of the "processing" class that WooCommerce core uses to notify gateways / plugins that it's not safe to submit. We were adding the class too early. Our sequence now matches core WooCommerce.
    </li>
  </ul>
  <p>
    <strong>Version 2.4.7</strong>
  </p>
  <ul>
    <li>Minor JS fix to logged out Amazon Pay flow.
    </li>
  </ul>
  <p>
    <strong>Version 2.4.6</strong>
  </p>
  <ul>
    <li>Improve login detection user experience: When entering an email address that is not associated with a login, the create an account checkbox will always be visible, and will default to checked. (Unless of course registration is disabled.)
    </li>
    <li>Bug: Fixed minor glitch with PayPal Checkout for WooCommerce.
    </li>
    <li>Fixed styling issue with WooCommerce Germanized.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.4.5</strong>
  </p>
  <ul>
    <li>Fix Amazon Pay
    </li>
    <li>Fix Klarna Payments for logged in users.
    </li>
    <li>Fix how cart errors are displayed on page load.
    </li>
  </ul>
  <p>
    <strong>Version 2.4.4</strong>
  </p>
  <ul>
    <li>Improve compatibility with native WooCommerce UI blocker. (Fixes UX issue with PayPal for WooCommerce when using skip final details option)
    </li>
    <li>Don't allow themes or plugins to nuke checkout page background.
    </li>
    <li>Add separate Mexican translations with improved Spanish translations. (Props:&nbsp;Filiberto Flores&nbsp;ðŸ‘ðŸ»)
    </li>
  </ul>
  <p>
    <strong>Version 2.4.3</strong>
  </p>
  <ul>
    <li>NEW: Payment methods and place order container are now dynamically refreshed on update_checkout event. This more closely matches how core does their fragment updates and allows for more advanced scenarios, such as conditionally showing gateways based on other conditions.
    </li>
    <li>Fix: Fixed JS error with footer text WYSIWYG on admin screen.
    </li>
    <li>Fix: PayPal Checkout for WooCommerce now works properly.&nbsp;
    </li>
    <li>Enhanced: Hardened our protections against WooCommerce loading its native stylesheets and scripts on the checkout page.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.4.2</strong>
  </p>
  <ul>
    <li>Enhanced: If shipping methods are available, show a normal shipping total instead of "Not Calculated", even when shipping hasn't been calculated.&nbsp;
    </li>
    <li>Enhanced: Rework theme compatibility protections for wp_footer hook to support configurations where output buffering is disabled or not working due to other themes or plugins.&nbsp;
    </li>
    <li>Fix: Fix edge case JavaScript error when directly loading the shipping method tab by URL.
    </li>
  </ul>
  <p>
    <strong>Version 2.4.1</strong>
  </p>
  <ul>
    <li>Fix: Fix another issue with plugins that load old versions of Kint.
    </li>
    <li>Fix: Password placeholder is now translated properly in themes.
    </li>
    <li>Fix: CheckoutWC child templates can load their styles and scripts properly.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.4.0</strong>
  </p>
  <p>
    <strong>WARNING:</strong>This release improves compatibility with other plugins, but consequently makes it more possible for themes and plugins to introduce problems. Please test and be prepared to rollback to 2.3.0 if you have significant problems. <a href="https://www.dropbox.com/s/n19t9c3unqb3xqs/checkout-for-woocommerce-2.3.0.zip?dl=0">You can download a copy of 2.3.0 here</a>.
  </p>
  <ul>
    <li>NEW: Fully working Customizer support! You can now change design settings from the front end and see what they look like in real time.
    </li>
    <li>NEW: Add support for wp_head and wp_footer to increase support for third party plugins!
    </li>
    <li>FIX: Google Analytics Integration now works correctly.&nbsp;
    </li>
    <li>FIX: Email placeholder is now properly translated.&nbsp;
    </li>
    <li>FIX: Address Line 2 is now properly translated.
    </li>
    <li>FIX: Amazon Pay button logo now shows up properly.
    </li>
    <li>ENHANCED: Instead of showing "Free!", shipping will now read "Not Calculated" when shipping has not been calculated and "Not Available" when no shipping methods are available.
    </li>
    <li>FIX: Fix styling of breadcrumbs on Copify template when viewing mobile styles on desktop browser.
    </li>
    <li>FIX: Fix fatal error when older version of Kint is loaded by another plugin or theme.
    </li>
    <li>NEW: Add&nbsp;cfw_enable_zip_autocomplete filter to disable zip auto lookup. Automatically disable zip auto lookup when Checkout Address Autocomplete is activated.&nbsp;
    </li>
    <li>FIX: Add stricter styling to prevent gateways like Stripe from messing up our styling.
    </li>
    <li>FIX: Add compatibility class for Avada theme to prevent it from wrecking checkout page styles.
    </li>
    <li>FIX: Fixed bug where create an account checkbox could be checked and active but hidden, leading to unexpected errors.
    </li>
    <li>NEW: Added support for ToCheckoutCW, a 2Checkout gateway plugin.
    </li>
    <li>ENHANCED: Move billing address fields above payment fields so that gateways that reset on update_checkout don't cause users to have to do double work.
    </li>
    <li>NEW: Support for Klarna Payments
    </li>
    <li>NEW: Persist payment method selection in the sessions.&nbsp;
    </li>
    <li>NEW: Added cfw_checkout_after_payment_tab_billing_address action.
    </li>
  </ul>
  <p>
    <strong>Version 2.3.0</strong>
  </p>
  <ul>
    <li>New - Added support for Klarna gateway.
    </li>
    <li>New - Added beta support for AfterPay gateway.
    </li>
    <li>Fix - Don't fire checkout_errors JS event on success messages. This caused issues with Klarna, and possibly other gateways.&nbsp;
    </li>
    <li>Improved - Refactored alerts to have three flavors: warnings, errors, success
    </li>
    <li>Improved - Added email address to "Welcome back" text for logged in users.&nbsp;
    </li>
    <li>Improved - Login / registration settings now obey the WooCommerce -&gt; Settings -&gt; Account screen.&nbsp;
    </li>
    <li>Improved - Added cancel button so that users can logout of PayPal Express (with PayPal for WooCommerce - Angelleye gateway)
    </li>
    <li>Improved - Added notice after PayPal Express login so that users know to continue with checkout.
    </li>
  </ul>
  <p>
    <strong>Version 2.2.5</strong>
  </p>
  <ul>
    <li>FIX - We changed the submit button in 2.2.3 to an &lt;input&gt;, which caused some orders to double submit. This was a huge screw up and we are so sorry to anyone who installed 2.2.3 or 2.2.4 today and experienced this issue.
    </li>
  </ul>
  <p>
    <strong>Version 2.2.4</strong>
  </p>
  <ul>
    <li>Fixed - JS errors in console when registration is required.
    </li>
    <li>Improved - Added setting to General tab to enable phone fields.
    </li>
  </ul>
  <p>
    <strong>Version 2.2.3</strong>
  </p>
  <ul>
    <li>Fixed - Billing address heading no longer shows up when using Amazon Pay.&nbsp;
    </li>
    <li>Improved - Submit button is now a button and not a link, in case plugins or gateways expect it to be one.
    </li>
    <li>Improved - Wording for login and account creation is now simpler. Checkbox for account creation is not shown if registration is mandatory.
    </li>
    <li>Improved - Prevent conflicts between Woo Checkout Field Editor and Checkout Manager. (These plugins are still incompatible with CheckoutWC)
    </li>
    <li>Fixed - SkyVerge gateways using latest SkyVerge payment gateway framework now load their scripts properly.
    </li>
    <li>New - Added support for Cielo gateway.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.2.2</strong>
  </p>
  <ul>
    <li>ðŸš¨IMPORTANT FIX: WooCommerce 3.5 changed how they loaded payment gateways so that under some circumstances, gateways were not loaded before CheckoutWC's template was loaded, breaking Stripe and probably other gateways. This release fixes this issue!
    </li>
    <li>Fixed styling of Mailchimp for WooCommerce checkboxes.&nbsp;
    </li>
    <li>Fixed styling of paragraph tags in terms and conditions box.
    </li>
    <li>Added class "secure-notice" to all transactions are secure notice.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.2.1</strong>
  </p>
  <ul>
    <li>Fixed bug with WooCommerce Subscriptions when only one shipping method is available.
    </li>
    <li>Fixed styling bug with Copify and Midas themes and WooCommerce Subscriptions shipping methods.&nbsp;
    </li>
    <li>Simplified PayPal for WooCommerce availability check to increase performance.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.2.0</strong>
  </p>
  <ul>
    <li>Added support for Crafty Clicks.&nbsp;
    </li>
    <li>Added support for shipped WooCommerce Subscriptions.&nbsp;
    </li>
    <li>Fixed styling glitch on template settings tab.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.1.6</strong>
  </p>
  <ul>
    <li>Add support for WooCommerce Google Analytics Integration&nbsp;ðŸ“ˆ
    </li>
    <li>Add support for WooCommerce Hear About Us&nbsp;ðŸŽ§
    </li>
    <li>Fix bug where Stripe greedily removes separator when PayPal Express button is visible.&nbsp;ðŸ›
    </li>
  </ul>
  <p>
    <strong>Version 2.1.5</strong>
  </p>
  <ul>
    <li>Prevent plugins from re-ordering post code field in such a way that it breaks the layout.&nbsp;
    </li>
    <li>Add beta support for WooCommerce Germanized. Feedback welcome!
    </li>
  </ul>
  <p>
    <strong>Version 2.1.2/2.1.3/2.1.4</strong>
  </p>
  <ul>
    <li>Tweaks to Futurist theme style
    </li>
    <li>Tweak to Payment Button margins
    </li>
    <li>Tweak to Copify template top margins
    </li>
    <li>Fix breadcrumb font sizes on mobile
    </li>
    <li>Update support beacon to include documentation search and live chat
    </li>
  </ul>
  <p>
    <strong>Version 2.1.1</strong>
  </p>
  <ul>
    <li>Payment buttons are now consistently styled for Amazon Pay, PayPal Express, Payment Requests (Chrome) and Apple Pay
    </li>
    <li>Styling fixes on mobile and desktop for several of the themes.
    </li>
    <li>Fixed glitch with Login auto detection. When a user clicks the Login link, the login form will stay open even if they put in an email address that is not a valid login.
    </li>
    <li>Optimized composer autoloader&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 2.1.0</strong>
  </p>
  <ul>
    <li>Support for Pakkalabels for WooCommerce&nbsp;ðŸ“¦
    </li>
    <li>Fixed bug with payment request buttons in Futurist theme.&nbsp;ðŸ•·
    </li>
  </ul>
  <p>
    <strong>Version 2.0.1/2.02</strong>
  </p>
  <ul>
    <li>Fixed a bug with the logo positioning in the Futurist theme.
    </li>
    <li>Fixed bug with load order that caused filters in theme functions.php to not be used.
    </li>
  </ul>
  <p>
    <strong>Version 2.0.0</strong>
  </p>
  <ul>
    <li>ðŸ“£&nbsp;Major release! There are potentially some breaking changes here, so please read the release notes thoroughly!
    </li>
    <li>ðŸ–¼&nbsp;Multiple templates! In addition to the default template, we have two new templates:
      <ul>
        <li>Copify - A theme styled to look as much like Shopify as possible.
        </li>
        <li>Futurist - A fresh theme with a slightly different vibe.
        </li>
        <li>Midas - The classic, default theme.
        </li>
      </ul>
    </li>
  </ul>
  <ul>
    <li>Design settings are now specific to the template, so you can safely change templates without eliminating you current settings.&nbsp;ðŸŽ¨
    </li>
    <li>If you have overridden the template files in your WordPress child theme, your template will still work. However it's important to update your template files as soon as possible as this functionality will be removed in a future release!&nbsp;âš&nbsp;
    </li>
    <li>Payment buttons like Apple Pay and Google Payment Request&nbsp;(both through Stripe) and PayPal Express are shown at the beginning of checkout, in a nicely formatted way that makes it easy to enable all three options.&nbsp;ðŸ’¸
    </li>
    <li>Added support for Braintree!&nbsp;â­ï¸
    </li>
    <li>Added support for Amazon Pay!â­ï¸
    </li>
    <li>Fixed compatibility issue with Pixel Your Site Pro.&nbsp;ðŸ•·
    </li>
    <li>Added support for Facebook for WooCommerce.&nbsp;âœ…
    </li>
    <li>Fixed bug with WooCommerce subscriptions.ðŸ•·
    </li>
  </ul>
  <p>
    <strong>Version 1.6.1</strong>
  </p>
  <ul>
    <li>Remove invasive styling overrides on Stripe form. Let default layout reign supreme.
    </li>
  </ul>
  <p>
    <strong>Version 1.6.0</strong>
  </p>
  <ul>
    <li>Tweak: Hide taxes from totals area when taxes are disabled.&nbsp;
    </li>
    <li>Fix: Change shipping address summary to use internationalized field labels.&nbsp;
    </li>
    <li>Added: Beta support for <a href="https://wordpress.org/plugins/paypal-for-woocommerce/">PayPal for WooCommerce</a>'s PayPal gateways.&nbsp;
    </li>
    <li>Tweak: Imported default WooCommerce form layout styling to better support default gateway styling and removed per gateway styling for Authorize.net AIM/CIM, PayPal Express/Pro/PayFlowPro.
    </li>
    <li>Tweak: Don't use constant to pass translation domain to keep with best practices.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 1.5.7</strong>
  </p>
  <ul>
    <li>Fixed bug with Chrome in Android that caused the mobile details widget to close when focusing on the promo field.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 1.5.6</strong>
  </p>
  <ul>
    <li>Fix MixPanel JS output position to fix JS error.
    </li>
  </ul>
  <p>
    <strong>Version 1.5.5</strong>
  </p>
  <ul>
    <li>Add back ability to remove a coupon from checkout page.&nbsp;
    </li>
    <li>Add support for Portuguese language translation.&nbsp;
    </li>
    <li>Update debugging library Kint to 2.x to prevent conflicts with other installs.
    </li>
  </ul>
  <p>
    <strong>Version 1.5.4</strong>
  </p>
  <ul>
    <li>Added&nbsp;cfw_show_shipping_tab filter. Allows the shipping method tab to be hidden arbitrarily by developers.
    </li>
    <li>Fixed payment icon display in recent versions of Stripe 4.1.x
    </li>
  </ul>
  <p>
    <strong>Version 1.5.3</strong>
  </p>
  <ul>
    <li>Fixed conflict between apply coupon AJAX endpoint and WooCommerce's native coupon AJAX handler.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 1.5.2</strong>
  </p>
  <ul>
    <li>Add support for AutomateWoo 3.7+.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 1.5.1</strong>
  </p>
  <ul>
    <li>Correct display of shipping methods when a single shipping method is available.
    </li>
    <li>Fix issue with taxes not being displayed in itemized totals.&nbsp;
    </li>
    <li>Added retool trigger on zip change for faster performance.
    </li>
  </ul>
  <p>
    <strong>Version 1.5.0</strong>
  </p>
  <ul>
    <li>Added support for First Data gateway:
      <ul>
        <li>Payeezy
        </li>
        <li>Payeezy JS
        </li>
        <li>Global Gateway
        </li>
      </ul>
    </li>
    <li>Improved styling of Authorize.net CIM fields
    </li>
    <li>Removed .gitignore file from output build to prevent problems with including plugin in a git repository.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 1.4.0</strong>
  </p>
  <ul>
    <li>Added support for WooCommerce shipping packages.ðŸ“¦&nbsp;
    </li>
    <li>Also works with WooCommerce Advanced Shipping Packages!
    </li>
  </ul>
  <p>
    <strong>Version 1.3.2</strong>
  </p>
  <ul>
    <li>Added - Support for WooCommerce Square payment gateway.
    </li>
    <li>Added -&nbsp;cfw_create_account_checkbox_label filter to filter label of create account checkbox.
    </li>
    <li>Fixed - When a customer switched countries from the default country, the state was not properly sent on submit.
    </li>
  </ul>
  <p>
    <strong>Version 1.3.1</strong>
  </p>
  <ul>
    <li>Fixed bug with One Click Upsell's Stripe gateway and the compatibility module refactors.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 1.3.0</strong>
  </p>
  <p>
    In no particular order:
  </p>
  <ul>
    <li>Refactored all compatibility classes for plugins and gateways into a new, easily maintainable structure.&nbsp;ðŸ†
    </li>
    <li>Improved Stripe gateway support robustness.&nbsp;ðŸ’ª
    </li>
    <li>Deprecated support for Stripe 3.x. Please use Stripe 4.x.&nbsp;
    </li>
    <li>Fixed bug with Jilt integration not tracking recovered purchases.
    </li>
    <li>Added spinner to overlay and improved overlay display.
    </li>
    <li>Fixed bug with international addresses.
    </li>
    <li>Fixed bug with account exists AJAX check.
    </li>
    <li>Moved all AJAX endpoints to wc_ajax from wp_ajax. (Related to Jilt fix)
    </li>
    <li>Added support for:&nbsp;âœ…
      <ul>
        <li>Google Analytics Pro
        </li>
        <li>Enhanced Ecommerce Google Analytics for WooCommerce
        </li>
        <li>WooCommerce Points and Rewards
        </li>
        <li>WooCommerce One Page Checkout
        </li>
        <li>Pixel Cat
        </li>
        <li>AutomateWoo
        </li>
      </ul>
    </li>
  </ul>
  <p>
    <strong>Version 1.2.4.1</strong>
  </p>
  <ul>
    <li>Hotfix to remove leftover type hints in path manager class that could cause fatal errors on activation for users in particular PHP environments.
    </li>
  </ul>
  <p>
    <strong>Version 1.2.4</strong>
  </p>
  <ul>
    <li>Fixed bug with Stripe 4.x on mobile that could prevent orders from successfully completing.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 1.2.3</strong>
  </p>
  <ul>
    <li>Added support for Stripe gateway embedded in One Click Upells from WooCurve. Also supports PayPal implementation.
    </li>
  </ul>
  <p>
    <strong>Version 1.2.2</strong>
  </p>
  <ul>
    <li>Fixed edge case bug where registration password override prevented creating an account on account page. Now only applies on checkout page.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 1.2.1</strong>
  </p>
  <ul>
    <li>BUG: Fix issue where "Same as Shipping" radio button resulted in billing field errors.&nbsp;
    </li>
    <li>BUG: Fix issue where "View cart" button could be hijacked with checkout url.&nbsp;
    </li>
    <li>BUG: Fix issue where JS error was possible on checkout page.
    </li>
    <li>BUG: Fix issue where billing phone was required even though phone fields were disabled.
    </li>
    <li>BUG: Fix issue where double or triple clicking submit could result in multiple orders.
    </li>
    <li>BUG: Fix issue where "Create Account" checkbox did not result in an account being created.
    </li>
    <li>ENHANCEMENT: Remove link underline on header logo area.&nbsp;
    </li>
    <li>FEATURE: Add support for Authorize.net CIM
    </li>
  </ul>
  <p>
    <strong>Version 1.2.0</strong>
  </p>
  <ul>
    <li>We refactored our submission model to work with more gateways out of the box.&nbsp;ðŸ—
    </li>
    <li>Stripe 4.x gateway support! (Backwards compatible with Stripe 3.x)&nbsp;ðŸ’³
      <ul>
        <li>AND! Stripe Checkout (modal)&nbsp;
        </li>
        <li>ALSO: Bancontact, SOFORT, Giropay, iDeal, P24, Alipay, SEPA Direct Debit, etc
        </li>
      </ul>
    </li>
    <li>BlueSnap gateway support&nbsp;ðŸ’³
    </li>
    <li>Phone fields support (<a href="https://gist.github.com/clifgriffin/39c615e586f7e0b33eb430c56e87aab0">added with filter</a>)&nbsp;ðŸ“ž
    </li>
    <li>Notes field support (<a href="https://gist.github.com/clifgriffin/1f8f441e47ccc72675ff9cc394322b2f">added with filter</a>)&nbsp;ðŸ“
    </li>
  </ul>
  <p>
    <strong>Version 1.1.5</strong>
  </p>
  <ul>
    <li>Fixed a small bug with the add-to-cart URL parameter where normal Add to Cart requests were redirected to checkout instead of the cart. Thanks, Scott! ðŸ‘ðŸ¼
    </li>
  </ul>
  <p>
    <strong>Version 1.1.4</strong>
  </p>
  <ul>
    <li>Added support for Checkout Address Autocomplete (<a href="https://wordpress.org/plugins/checkout-address-autocomplete-for-woocommerce/">https://wordpress.org/plugins/checkout-address-autocomplete-for-woocommerce/</a>)
    </li>
  </ul>
  <p>
    <strong>Version 1.1.3</strong>
  </p>
  <ul>
    <li>Added basic "Checkout Loads" test support for Robot Ninja (<a href="https://robotninja.com/">https://robotninja.com</a>)
    </li>
  </ul>
  <p>
    <strong>Version 1.1.2</strong>
  </p>
  <ul>
    <li>ðŸ•·Fixed bug with variation combination not showing up in cart line items.
    </li>
    <li>â­&nbsp;Added support for add-to-cart={product_id} URL parameter. So you can pre-load the cart for checkout with a URL like: <a href="https://demo.checkoutwc.com/checkout/?add-to-cart=56">https://demo.checkoutwc.com/checkout/?add-to-cart=56</a>
    </li>
  </ul>
  <p>
    <strong>Version 1.1.1</strong>
  </p>
  <ul>
    <li>Fix bug with Apple Pay separator showing up in Chrome and other browsers.
    </li>
  </ul>
  <p>
    <strong>Version 1.1.0</strong>
  </p>
  <ul>
    <li>Added support for Tickera tickets with Bridge for WooCommerce
    </li>
    <li>Added support for Redsys Gateway
    </li>
    <li>Added support for PayPal Express
    </li>
    <li>Improved styling of separator between Apple Pay / PayPal Express and customer info.&nbsp;
    </li>
    <li>Fix bug where checkout template overrides order-pay checkout endpoint.&nbsp;
    </li>
  </ul>
  <p>
    <strong>Version 1.0.4</strong>
  </p>
  <ul>
    <li>Fix internationalization issue with geolocation and state label.
    </li>
    <li>Fix safari bug on successful order.
    </li>
  </ul>
  <p>
    <strong>Version 1.0.3</strong>
  </p>
  <ul>
    <li>Fix IE 11 compatibility issues.&nbsp;
    </li>
    <li>Add warning for Stripe Gateway 4.x.
    </li>
    <li>Update translations.
    </li>
  </ul>
  <p>
    <strong>Version 1.0.2</strong>
  </p>
  <ul>
    <li>Add license notice to settings screen.
    </li>
    <li>Add return to cart button to customer information tab.
    </li>
    <li>Add cart breadcrumb to header links.
    </li>
    <li>Link logo to homepage.
    </li>
  </ul>
  <p>
    <strong>Version 1.0.1</strong>
  </p>
  <ul>
    <li>Fix bug where payment fields do not show up for orders that need payment.
    </li>
  </ul>
  <p>
    <strong>Version 1.0.0</strong>
  </p>
  <ul>
    <li>We have a release!&nbsp;ðŸ¾ðŸŽ‰ðŸ™Œ
    </li>
  </ul>
