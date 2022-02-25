---
title: How to Install CheckoutWC With Composer
slug: how-to-install-checkoutwc-with-composer
cats: How To
---

 If you're a developer who loves managing dependencies with Composer (we certainly do) you can install CheckoutWC with composer. Here are the steps!

Add Our Repository
------------------

```
{
	"repositories": [
		{
			"type": "composer",
			"url": "https://www.checkoutwc.com/composer/{YourLicenseKey}"
		}
	]
}
```

 Substitute {YourLicenseKey} with your actual license key.

Add Our Plugin
--------------

 From your CLI (terminal) run: ```
composer require objectivco/checkout-for-woocommerce
```

Version Constraints
-------------------

 You can use any [Composer version constraints](https://getcomposer.org/doc/articles/versions.md), or specify the exact version of a plugin or addon:

```
"require": {
    "objectivco/checkout-for-woocommerce": "3.7.1"
}
```

Example composer.json
---------------------

```
{
    "name": "your/project",
    "description": "A CheckoutWC site",
    "repositories": [
       {
		"type": "composer",
		"url": "https://www.checkoutwc.com/composer/123456890"
	}
    ],
    "require": {
        "objectivco/checkout-for-woocommerce": "^3.7"
    }
}
```