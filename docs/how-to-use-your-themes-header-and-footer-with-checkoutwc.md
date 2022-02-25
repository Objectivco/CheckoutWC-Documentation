---
title: How to Use Your Theme's Header and Footer with CheckoutWC
slug: how-to-use-your-themes-header-and-footer-with-checkoutwc
cats: How To
---

We don't load the theme's header and footer for a couple of important reasons:

1. The typical site header includes lot of links, menus, and other things that can be distracting and lower conversions. We designed the checkout page to feel like a separate area of the site, intended for some thing: purchasing
2. Loading the theme header and footer requires loading theme styles, which increases the risk of conflicts.

Using Your Theme's Header and Footer
------------------------------------

If you would like to customize CheckoutWC to use your theme's footer and header you have four options.
### Option 1) Elementor Pro

 If you're an Elementor Pro user, you're in luck! Simple head to **Settings** &gt; **Integrations** and click the checkbox next to 'Enable Elementor Pro support.'

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e90bfae2c7d3a7e9aeac421/file-geBMgYhdnf.png)

When this setting is enabled, we'll pull in the header and footer you have configured with Elementor Pro.
You'll need to configure the display options to have it show up either Site Wide or on the checkout page specifically. These settings are displayed when saving a the module:
![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5ee8d05b04286306f8053b21/file-PJrJvWV68R.jpg)


### Option 2) Beaver Theme

 If you're using Beaver Builder and have their Beaver Themer add-on, you can configure a header and footer module and set it to display on the checkout page. You'll need to activate the Beaver Themer integration:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5ee8d0b72c7d3a10cba8fd18/file-Ovm9PUAZdR.png)

### Option 3) Experimental Template Loader

 Starting in 3.6, we added a setting that allows you to load the CheckoutWC template inside of your WordPress theme.

 This is an experimental feature and is NOT supported. You will likely have styling and other issues and we cannot provide support for problems caused by this configuration.

 But if you have are a developer or have access to one who can solve these issues, it is an option.

 To enable to go to Settings &gt; CheckoutWC &gt; Integrations and switch 'Template Loader' to WordPress Theme:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5eed25d12c7d3a10cba94354/file-ZTitKs5egG.png)

### Option 4) Custom coding

Option 4 is a little less straightforward, but if you are a developer (or have access to a developer), you should be able to do it without too much pain.
There are two main strategies:
1. Use action hooks
2. Create a custom template

 We recommend using the action hook strategy wherever possible.

 For instance, to add a custom header you could do something like this:

<script src="https://gist.github.com/clifgriffin/cb9277da01133d89717be736d1435c59.js" type="text/javascript"></script> That will add a custom header with styling, as well as hide the default header.

 If you would like to do something more custom, you can try your hand at creating a [custom template](https://kb.checkoutwc.com/article/24-template-files). **However we really recommend you do this as a last resort.** Maintaining a custom template will require a lot more time in the long run than using action hooks and you should be able to do anything you need to do with action hooks.
