---
title: SmartyStreets Address Validation
slug: smartystreets-address-validation
cats: Features
---

 Address Validation looks up the shipping address entered by your customer and attempts to verify that it is the correct address using SmartyStreets Address APIs.

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60ae79392246b50b7f38f49e/file-csXMvkJ81K.gif)

 Like many features, we encourage merchants to be cautious about enabling functionality like this. Requiring a customer to validate the address they entered adds some additional friction to the checkout process and could result in lower conversions.

 We encourage merchants to enable this feature if they have regular issues with failed orders due to incorrect address entry.

Configuration
-------------

 To setup SmartyStreets, you'll need a SmartyStreets account:

 <https://www.smartystreets.com/pricing>

 If all of your customers are based in the United States, you can purchase a US Address plan. If you have low volume, you can use their free tier which includes 250 lookups a month.

 If you are not based in the US or sell to multiple countries, you'll also need their International Address API:

 <https://www.smartystreets.com/pricing/international>

 Once you have signed up for the required APIs, you can login to SmartyStreets and access your API Keys:

 <https://www.smartystreets.com/account/keys>

 You'll want to generate a Secret Key which looks like this:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60ae7a9c4dda6972e092f74d/file-y9hjoOJLaI.png)

 You'll enter those keys in **WP Admin &gt; CheckoutWC &gt; Checkout**:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60ae7b25c1410a601d9ad311/file-hobElCJaNc.png)

Considerations and Edge-cases
-----------------------------

### Precision

 Addresses are complex and sometimes even a first-class validation service like SmartyStreets can't verify an address completely. SmartyStreets indicates how precisely it verifies an address. Occasionally SmartyStreets will say it can only verify an address down to the "Locality," meaning it's only confident that the city, state, and country etc are correct. When this occurs we lean towards trusting the user to correctly input their address and we won't show them a confirmation popup.

### United Kingdom

 The United Kingdom's addresses are such that sometimes cities or neighborhoods are suggested for address line 2. Because of this we check to make sure the SmartyStreets suggestion for Address Line 2 isn't a duplicate of another component already in the address.

 The United Kingdom's addresses are also such that sometimes the Address Line 1 and Address Line 2 are the reverse of how we would normally expect them to be in the US and how WooCommerce would expect. Example: Apt 20 may end up in address\_1 and "10 Downing St" in address\_2.

Unfortunately these are the foibles of addresses and particularly UK addresses. If this causes problems for your customers and you have a lot of UK customers, you may wish to disable the feature.

 Frequently Asked Questions
---------------------------

### What happens when I run out of lookups?

 If you run out of lookups, address validation should fail silently and the user will be advanced to the next step without having to verify their address.