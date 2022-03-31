---
title: Configuring Avada to Work With CheckoutWC
slug: avada-template-layout-problems
cats: Troubleshooting
---

<p>Configuring Avada to work well with CheckoutWC requires changing two options.</p>
<h4>Step 1) Go to Avada &gt; Options</h4>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60c765d3af164f7b537cdfdd/file-usaYMc7RSA.png" alt="" /></p>
<h4>Step 2) Search for 'WooCommerce One Page Checkout' in the settings search and turn the feature to Off.</h4>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5cb698cc2c7d3a07c44a1ae1/file-xLZ86BnNAN.png" alt="" /></p>
<h4>Step 3) Search for 'CSS Compiling Method' in the setting search and turn the feature to Disabled.</h4>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/60c765feaf164f7b537cdfdf/file-fx2nqbZTKK.png" alt="" /></p>
<h3>Step 4) Search for 'Enable JS Compiler' and turn it to Off</h3>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/622b5dccab585b230a89f9f9/file-h70tI55p9i.png" alt="" /></p>
<p>Most servers use HTTP/2 these days so combining JS or CSS files is generally an anti-pattern and can cause poorer performance.</p>
<h4>Step 4) Save Settings</h4>
