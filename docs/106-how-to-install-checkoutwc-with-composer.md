---
title: How to Install CheckoutWC With Composer
slug: how-to-install-checkoutwc-with-composer
cats: How To
status: published
---


  <p>
    If you're a developer who loves managing dependencies with Composer (we certainly do) you can install CheckoutWC with composer. Here are the steps!
  </p>
  <h2>
    Add Our Repository
  </h2>
  <pre>{
        "repositories": [
                {
                        "type": "composer",
                        "url": "https://www.checkoutwc.com/composer/{YourLicenseKey}"
                }
        ]
}
</pre>
  <p>
    Substitute {YourLicenseKey} with your actual license key.
  </p>
  <h2>
    Add Our Plugin
  </h2>
  <p>
    From your CLI (terminal) run:
  </p>
  <pre>composer require objectivco/checkout-for-woocommerce
</pre>
  <h2>
    Version Constraints
  </h2>
  <p>
    You can use any <a href="https://getcomposer.org/doc/articles/versions.md" target="_blank">Composer version constraints</a>, or specify the exact version of a plugin or addon:
  </p>
  <pre>"require": {
    "objectivco/checkout-for-woocommerce": "3.7.1"
}
</pre>
  <h2>
    Example composer.json
  </h2>
  <pre>{
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
</pre>
