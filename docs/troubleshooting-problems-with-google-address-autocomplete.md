---
title: Troubleshooting Problems with Google Address Autocomplete
slug: troubleshooting-problems-with-google-address-autocomplete
cats: Troubleshooting
---

 If there's a problem with your Google API key you will see something like this on your checkout page:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6202a5dad86136157d9a20d3/file-oDNJ7yjouK.png)

 This indicates that there's a problem with your Google API Key. This isn't a CheckoutWC issue.

 To determine what the problem is, [open up your browser's developer tools](https://kb.checkoutwc.com/article/146-how-to-access-your-browsers-developer-tools-for-debugging) and check the console for a log entry like this:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6202a73b68cd260cc2d38faf/file-APMTqS5on6.png)

Most common problems:
---------------------

1. The API key is not allowed on the current site. (RefererNotAllowedMapError)
2. The API key doesn't have access to the necessary APIs. (Maps, Places, Geocoding)
3. The project doesn't have access to the necessary APIs (Maps, Places, Geocoding)
4. Your Google Cloud Project doesn't have billing enabled.