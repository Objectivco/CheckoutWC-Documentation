---
title: Generate Password Filter
slug: generate-password-filter
cats: Developers
---

 If WooCommerce settings allow for creating accounts while checking out we will generate a password for users who don't have an account.

 You can override this functionality in your child theme's functions.php file with the filter below.

```php
add_filter( 'cfw_registration_generate_password', '__return_false' );
```
