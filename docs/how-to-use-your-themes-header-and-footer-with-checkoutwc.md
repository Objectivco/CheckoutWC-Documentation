---
title: How to Use Your Theme's Header and Footer with CheckoutWC
slug: how-to-use-your-themes-header-and-footer-with-checkoutwc
cats: How To
---


  <div>
    We don't load the theme's header and footer for a couple of important reasons:&nbsp;<br />
    <ol>
      <li>The typical site header includes lot of links, menus, and other things that can be distracting and lower conversions. We designed the checkout page to feel like a separate area of the site, intended for some thing: purchasing
      </li>
      <li>Loading the theme header and footer requires loading theme styles, which increases the risk of conflicts.&nbsp;
      </li>
    </ol>
    <h2>
      Using Your Theme's Header and Footer
    </h2>
    <div>
      If you would like to customize CheckoutWC to use your theme's footer and header you have four options.
    </div>
    <h3>
      Option 1) Elementor Pro
    </h3>
    <p>
      If you're an Elementor Pro user, you're in luck! Simple head to <strong>Settings</strong> &gt; <strong>Integrations</strong> and click the checkbox next to 'Enable Elementor Pro support.'
    </p>
    <p>
      <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e90bfae2c7d3a7e9aeac421/file-geBMgYhdnf.png" />
    </p>
    <div>
      When this setting is enabled, we'll pull in the header and footer you have configured with Elementor Pro.
    </div>
    <div>
      You'll need to configure the display options to have it show up either Site Wide or on the checkout page specifically. These settings are displayed when saving a the module:
    </div>
    <div>
      <p>
        <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5ee8d05b04286306f8053b21/file-PJrJvWV68R.jpg" />
      </p>
    </div>
    <h3>
      Option 2) Beaver Theme
    </h3>
    <p>
      If you're using Beaver Builder and have their Beaver Themer add-on, you can configure a header and footer module and set it to display on the checkout page. You'll need to activate the Beaver Themer integration:
    </p>
    <p>
      <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5ee8d0b72c7d3a10cba8fd18/file-Ovm9PUAZdR.png" />
    </p>
    <h3>
      Option 3) Experimental Template Loader
    </h3>
    <p>
      Starting in 3.6, we added a setting that allows you to load the CheckoutWC template inside of your WordPress theme.
    </p>
    <p>
      This is an experimental feature and is NOT supported. You will likely have styling and other issues and we cannot provide support for problems caused by this configuration.
    </p>
    <p>
      But if you have are a developer or have access to one who can solve these issues, it is an option.
    </p>
    <p>
      To enable to go to Settings &gt; CheckoutWC &gt; Integrations and switch 'Template Loader' to WordPress Theme:
    </p>
    <p>
      <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5eed25d12c7d3a10cba94354/file-ZTitKs5egG.png" />
    </p>
    <h3>
      Option 4) Custom coding
    </h3>
    <div>
      Option 4 is a little less straightforward, but if you are a developer (or have access to a developer), you should be able to do it without too much pain.
    </div>
    <div>
      There are two main strategies:
    </div>
    <ol>
      <li>Use action hooks
      </li>
      <li>Create a custom template
      </li>
    </ol>
    <p>
      We recommend using the action hook strategy wherever possible.&nbsp;
    </p>
    <p>
      For instance, to add a custom header you could do something like this:
    </p>
    <script src="https://gist.github.com/clifgriffin/cb9277da01133d89717be736d1435c59.js" type="text/javascript"></script>
    <p>
      That will add a custom header with styling, as well as hide the default header.
    </p>
    <p>
      If you would like to do something more custom, you can try your hand at creating a <a href="https://cfw.staging.objectiv.co/documentation/template-files" target="_blank">custom template</a>. <strong>However we really recommend you do this as a last resort.</strong> Maintaining a custom template will require a lot more time in the long run than using action hooks and you should be able to do anything you need to do with action hooks.
    </p>
  </div>
