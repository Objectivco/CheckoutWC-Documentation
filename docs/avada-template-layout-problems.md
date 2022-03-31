---
title: Configuring Avada to Work With CheckoutWC
slug: avada-template-layout-problems
cats: Troubleshooting
---

 Configuring Avada to work well with CheckoutWC requires changing two options.

#### Step 1) Go to Avada &gt; Options

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60c765d3af164f7b537cdfdd/file-usaYMc7RSA.png)

####  Step 2) Search for 'WooCommerce One Page Checkout' in the settings search and turn the feature to Off.

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5cb698cc2c7d3a07c44a1ae1/file-xLZ86BnNAN.png)

#### Step 3) Search for 'CSS Compiling Method' in the setting search and turn the feature to Disabled.

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60c765feaf164f7b537cdfdf/file-fx2nqbZTKK.png)

### Step 4) Search for 'Enable JS Compiler' and turn it to Off

![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/622b5dccab585b230a89f9f9/file-h70tI55p9i.png)

Most servers use HTTP/2 these days so combining JS or CSS files is generally an anti-pattern and can cause poorer performance.

#### Step 4) Save Settings