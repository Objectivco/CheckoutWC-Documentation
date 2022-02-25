---
title: How to Add Custom Checkout Tabs
slug: how-to-add-custom-checkout-tabs
cats: How To
---

 Adding custom checkout tabs is possible, but takes some custom development to get working.

 Here is a 80% working demo of how you could add an Age Verification tab to the checkout process:

<script src="https://gist.github.com/clifgriffin/dbf6a26b2ee82787eac9a837f96f45d3.js" type="text/javascript"></script> What this code does:

- Adds an Age Verification link to the breadcrumb navigation
- Add an Age Verification tab to the tabs
- Adds tab navigation to the bottom of the Age Verification tab that takes you to the appropriate previous / next tabs
- Stubs out basic JavaScript to validate whether you can move to the next tab when you're on the age verification tab

 What this code doesn't do (the last 20%):

- It doesn't switch the navigation on the customer info and shipping method tabs to appropriately point the next and previous buttons to the correct tab. Here are the action hooks that add those navigations to the native tabs: <https://gist.github.com/clifgriffin/f7d090bbe66b6039c7cf57f88a1b0be3>
- The shipping tab can be hidden dynamically based on whether the cart has shipped items. This snippet doesn't handle that condition. You would need to have two next buttons on the age verification tab and use this CSS class to determine which to show: cfw-hide-shipping
- It doesn't actually add any age verification form control to the tab. (It's just an example after all!)

Hopefully this is helpful to get you started. Let us know if you get stuck.