---
title: International Phone Field
slug: international-phone-field
cats: Features
---

 The International Phone Field feature uses [international telephone input](https://intl-tel-input.com) to validate the phone number according to the country selected by the customer. It also allows you to format the phone number for normalized storage.

 **Requirements:**

1. **Pro** (10 Sites) or **Agency** (150 Sites) license
2. You must have [configured WooCommerce to enable the phone field](https://kb.checkoutwc.com/article/69-how-to-enable-billing-and-shipping-phone-fields).
3. For validation, the phone field must be required.

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/61648dc80332cb5b9e9b2a0a/file-0wBoibtOL0.png)

 By default, the phone field will be set the country the customer selected but it can be changed to a different country:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/61648e0c9ccf62287e5eac8e/file-6dcny0KTxT.png)

 If the phone field is required, a proper phone number must be entered for the selected country.

 The phone number can be stored in one of several formats:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/61648eb50332cb5b9e9b2a14/file-bZfmZse5BP.png)

**Raw Value:** The number is stored exactly how the user entered it.

**E164:** Format phone number with E164 standard.

**International:** Format phone number with RFC3966 standard without the tel: prefix

**National:** Format phone number based on selected country. US Example (555) 555 - 5555, UK Example: 07911 123457

**RFC3966:** Format phone number with RFC3966 standard.