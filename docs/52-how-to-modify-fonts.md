---
title: How To Customize Fonts
slug: how-to-modify-fonts
cats: How To
status: published
---


  <p>
    Checkout for WooCommerce uses the system font stack by default.&nbsp;
  </p>
  <p>
    This has the <a href="https://css-tricks.com/snippets/css/system-font-stack/">advantage of be lightning fast as well as well as matching the user's OS defaults</a>.&nbsp;
  </p>
  <h2>
    Using Google Fonts
  </h2>
  <p>
    To change your fonts, go to <strong>Settings</strong> &gt; <strong>CheckoutWC</strong> &gt; <strong>Design</strong> and change the the Body Font and Heading Font settings:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5e90c4b22c7d3a7e9aeac48b/file-tmOO1dt37a.png" />
  </p>
  <p>
    Then save your settings and you're good to go.
  </p>
  <h2>
    If your font list isn't loading.
  </h2>
  <p>
    Occasionally, our fetch to Google may return an error which gets cached as a transient. To fix this, try deleting all of your transients.
  </p>
  <p>
    With WP CLI you can use this:
  </p>
  <p>
    wp transient delete --all
  </p>
  <p>
    If you don't have access to WP CLI, you can use a plugin like this:
  </p>
  <p>
    <a href="https://wordpress.org/plugins/transients-manager/" target="_blank">https://wordpress.org/plugins/transients-manager/</a>
  </p>
  <h2>
    Using custom fonts.
  </h2>
  <p>
    If you can't find the font you need with Google Fonts, you can add a custom font. This will require custom coding.
  </p>
  <p>
    You can insert your style tags into <strong>Settings</strong> &gt; <strong>CheckoutWC</strong> &gt; <strong>General</strong> &gt; <strong>Header Scripts</strong>.
  </p>
  <p>
    We can't really help with this part, but if you run into a snag you're welcome to contact support and we'll try to point you in the right direction.
  </p>
