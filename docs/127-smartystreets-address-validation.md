---
title: SmartyStreets Address Validation
slug: smartystreets-address-validation
cats: Features
status: published
---


  <p>
    Address Validation looks up the shipping address entered by your customer and attempts to verify that it is the correct address using SmartyStreets Address APIs.
  </p>
  <p>
    <img style="max-width: 800px" src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60ae79392246b50b7f38f49e/file-csXMvkJ81K.gif" />
  </p>
  <p>
    Like many features, we encourage merchants to be cautious about enabling functionality like this. Requiring a customer to validate the address they entered adds some additional friction to the checkout process and could result in lower conversions.
  </p>
  <p>
    We encourage merchants to enable this feature if they have regular issues with failed orders due to incorrect address entry.
  </p>
  <h2>
    Configuration
  </h2>
  <p>
    To setup SmartyStreets, you'll need a SmartyStreets account:
  </p>
  <p>
    <a href="https://www.smartystreets.com/pricing">https://www.smartystreets.com/pricing</a>
  </p>
  <p>
    If all of your customers are based in the United States, you can purchase a US Address plan. If you have low volume, you can use their free tier which includes 250 lookups a month.
  </p>
  <p>
    If you are not based in the US or sell to multiple countries, you'll also need their International Address API:
  </p>
  <p>
    <a href="https://www.smartystreets.com/pricing/international">https://www.smartystreets.com/pricing/international</a>
  </p>
  <p>
    Once you have signed up for the required APIs, you can login to SmartyStreets and access your API Keys:
  </p>
  <p>
    <a href="https://www.smartystreets.com/account/keys">https://www.smartystreets.com/account/keys</a>
  </p>
  <p>
    You'll want to generate a Secret Key which looks like this:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60ae7a9c4dda6972e092f74d/file-y9hjoOJLaI.png" />
  </p>
  <p>
    You'll enter those keys in <strong>WP Admin &gt; CheckoutWC &gt; Checkout</strong>:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60ae7b25c1410a601d9ad311/file-hobElCJaNc.png" />
  </p>
  <h2>
    Considerations and Edge-cases
  </h2>
  <h3>
    Precision
  </h3>
  <p>
    Addresses are complex and sometimes even a first-class validation service like SmartyStreets can't verify an address completely. SmartyStreets indicates how precisely it verifies an address. Occasionally SmartyStreets will say it can only verify an address down to the "Locality," meaning it's only confident that the city, state, and country etc are correct. When this occurs we lean towards trusting the user to correctly input their address and we won't show them a confirmation popup.
  </p>
  <h3>
    United Kingdom
  </h3>
  <p>
    The United Kingdom's addresses are such that sometimes cities or neighborhoods are suggested for address line 2. Because of this we check to make sure the SmartyStreets suggestion for Address Line 2 isn't a duplicate of another component already in the address.
  </p>
  <p>
    The United Kingdom's addresses are also such that sometimes the Address Line 1 and Address Line 2 are the reverse of how we would normally expect them to be in the US and how WooCommerce would expect. Example: Apt 20 may end up in address_1 and "10 Downing St" in address_2.
  </p>
  <p>
    Unfortunately these are the foibles of addresses and particularly UK addresses. If this causes problems for your customers and you have a lot of UK customers, you may wish to disable the feature.
  </p>
  <h2>
    Frequently Asked Questions
  </h2>
  <h3>
    What happens when I run out of lookups?
  </h3>
  <p>
    If you run out of lookups, address validation should fail silently and the user will be advanced to the next step without having to verify their address.
  </p>
