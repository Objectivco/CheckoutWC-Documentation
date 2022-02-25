---
title: How To Register and Configure Your Google API Key
slug: how-to-get-and-configure-your-google-api-key
cats: How To
---

 There are two features that require a Google API Key to work properly:

1. [Address Autocomplete](https://kb.checkoutwc.com/article/72-how-to-enable-address-autocomplete)
2. Map Embed on the [Thank You Page](https://kb.checkoutwc.com/article/85-how-to-enable-and-configure-the-thank-you-page)

 In order to use these features, you need to register a Google API Key. You can do this through [Google's Cloud Platform](https://cloud.google.com/maps-platform/).

How To Register a Google API Key
--------------------------------

1. Visit <https://cloud.google.com/maps-platform/>
2. Click 'Get Started' in the top right
3. Select **Maps** and **Places**. Maps is required for the thank you page map embed. Places is required for the address autocomplete. It's generally preferable to register both, but if you do not wish to use one of these features you can select only the one you need. ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0bdae04286364bc9154d4/file-rwzZyt8s1e.png)
4. Select an existing project or create a new project: ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0be1b2c7d3a7e9ae38034/file-2kqobgT7XO.png)
5. Follow the steps to enable billing on your project. (For most users this should be free because Google provides a generous monthly credit, however we cannot answer questions about billing. You'll need to talk to Google!) Once you're through, you should be presented with your API key:![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0bf4f04286364bc9154de/file-FqIqgSgSkE.png)
6. Follow the link to go to the API Console.
7. Give your API Key a name and select HTTP Referrers under **Application Restrictions**. This allows you to restrict your key to just your site(s) for extra security. **This is very important or someone could steal your key and potentially abuse it, resulting in charges to your account! ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0c06504286364bc9154e9/file-qfLjTKBjha.png)**
8. If you choose to restrict the APIs your key can access, be sure to include Places API, Maps JavaScript API, and Geocoding API.
9. Once you have done the above, you should be good to go! Just add it to your settings under Settings &gt; CheckoutWC &gt; General &gt; Google API Key.

Troubleshooting
---------------

1. If you see exclamation points in the address field, open your browser's dev console. You will see an error message from Google indicating the problem preventing the APIs from loading.
2. The most common mistake is failing to enable the required APIs (Maps, Places, Geocoding) on both the Project and the API Key itself.