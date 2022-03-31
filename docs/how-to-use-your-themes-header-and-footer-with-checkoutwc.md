---
title: How to Use Your Theme's Header and Footer with CheckoutWC
slug: how-to-use-your-themes-header-and-footer-with-checkoutwc
cats: How To
---


<h2>Using Your Theme's Header and Footer</h2>

<p>If you're an Elementor Pro user, you're in luck! Simple head to <strong>Settings</strong> &gt; <strong>Integrations</strong> and click the checkbox next to 'Enable Elementor Pro support.'</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e90bfae2c7d3a7e9aeac421/file-geBMgYhdnf.png" alt="" /></p>


<p>If you're using Beaver Builder and have their Beaver Themer add-on, you can configure a header and footer module and set it to display on the checkout page. You'll need to activate the Beaver Themer integration:</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5ee8d0b72c7d3a10cba8fd18/file-Ovm9PUAZdR.png" alt="" /></p>
<h3>Option 3) Experimental Template Loader</h3>
<p>Starting in 3.6, we added a setting that allows you to load the CheckoutWC template inside of your WordPress theme.</p>
<p>This is an experimental feature and is NOT supported. You will likely have styling and other issues and we cannot provide support for problems caused by this configuration.</p>
<p>But if you have are a developer or have access to one who can solve these issues, it is an option.</p>
<p>To enable to go to Settings &gt; CheckoutWC &gt; Integrations and switch 'Template Loader' to WordPress Theme:</p>
<p><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5eed25d12c7d3a10cba94354/file-ZTitKs5egG.png" alt="" /></p>
<h3>Option 4) Custom coding</h3>

<p>We recommend using the action hook strategy wherever possible.</p>
<p>For instance, to add a custom header you could do something like this:</p>

<p>If you would like to do something more custom, you can try your hand at creating a <a href="https://kb.checkoutwc.com/article/24-template-files">custom template</a>. <strong>However we really recommend you do this as a last resort.</strong> Maintaining a custom template will require a lot more time in the long run than using action hooks and you should be able to do anything you need to do with action hooks.</p>
