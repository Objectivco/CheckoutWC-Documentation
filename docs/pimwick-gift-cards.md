---
title: Configure Pimwick Gift Cards to Work with CheckoutWC
slug: pimwick-gift-cards
cats: 3rd Party Themes and Plugins
---

 Pimwick Gift Cards has been tested and works with CheckoutWC properly.

 To have the best experience, you should use this option:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5f98394246e0fb0017991135/file-KKZhS5yaBK.png)

 "Below the Payment Methods Area" does NOT work. This is due to the plugin including a form tag which becomes nested within the checkout form and breaks the layout.

 HTML does not permit nested forms. This is a design flaw in the plugin so we recommend using the default location instead.