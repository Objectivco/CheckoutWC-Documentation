---
title: How to Bypass CheckoutWC for Testing
slug: how-to-bypass-checkoutwc-for-testing
cats: How To
---

If you need to test native WooCommerce checkout, you can do so without disabling CheckoutWC. Simply add this to your checkout URL: bypass-cfw=true

**Example:**

https://yoursite.com/checkout/?bypass-cfw=true

This is a great idea to do whenever you have a problem. This helps confirm the problem you are seeing is unique to CheckoutWC and not a general bug.