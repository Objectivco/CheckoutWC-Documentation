---
title: How To Add Country Restrictions to Address Autocomplete
slug: how-to-add-country-restrictions-to-address-autocomplete
cats: How To
---

 If you would like to restrict the countries that show up when using address autocomplete, you can use this snippet:

<script src="https://gist.github.com/clifgriffin/dddf4ddc25c55193c9535775bd375e49.js" type="text/javascript"></script>You must use 2 letter country abbreviations from the the ISO 3166-1 Alpha-2 standard:  
[https://en.wikipedia.org/wiki/ISO\_3166-1\_alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)

Note: Due to Google Maps API restrictions, they only accept 5 or fewer countries.