---
title: How To Change Validation Trigger for Billing Email (Or Other Fields)
slug: how-to-change-validation-trigger-for-billing-email-or-other-fields
cats: How To
---

 By default, the billing email validates on keyup. If you'd like to change it so it only validates after a user has finished filling out the field, you can use this example.

<script src="https://gist.github.com/clifgriffin/5503ea4374c190288e71058d61b45fdf.js" type="text/javascript"></script> To change other fields, you would use the same pattern but change the field group (billing) and field key (billing\_email) accordingly.