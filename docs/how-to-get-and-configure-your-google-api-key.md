---
title: How To Register and Configure Your Google API Key
slug: how-to-get-and-configure-your-google-api-key
cats: How To
---


  <p>
    There are two features that require a Google API Key to work properly:
  </p>
  <ol>
    <li>
      <a href="https://cfw.staging.objectiv.co/documentation/how-to-enable-address-autocomplete" target="_blank">Address Autocomplete</a>
    </li>
    <li>Map Embed on the <a href="https://cfw.staging.objectiv.co/documentation/how-to-enable-and-configure-the-thank-you-page" target="_blank">Thank You Page</a>
    </li>
  </ol>
  <p>
    In order to use these features, you need to register a Google API Key. You can do this through <a href="https://cloud.google.com/maps-platform/">Google's Cloud Platform</a>.
  </p>
  <h2>
    How To Register a Google API Key
  </h2>
  <ol>
    <li>Visit <a href="https://cloud.google.com/maps-platform/">https://cloud.google.com/maps-platform/</a>
    </li>
    <li>Click 'Get Started' in the top right
    </li>
    <li>Select <strong>Maps</strong>&nbsp;and <strong>Places</strong>. Maps is required for the thank you page map embed. Places is required for the address autocomplete. It's generally preferable to register both, but if you do not wish to use one of these features you can select only the one you need.&nbsp;<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0bdae04286364bc9154d4/file-rwzZyt8s1e.png" />
    </li>
    <li>Select an existing project or create a new project:&nbsp;<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0be1b2c7d3a7e9ae38034/file-2kqobgT7XO.png" />
    </li>
    <li>Follow the steps to enable billing on your project. (For most users this should be free because Google provides a generous monthly credit, however we cannot answer questions about billing. You'll need to talk to Google!) Once you're through, you should be presented with your API key:<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0bf4f04286364bc9154de/file-FqIqgSgSkE.png" />
    </li>
    <li>Follow the link to go to the API Console.&nbsp;
    </li>
    <li>Give your API Key a name and select HTTP Referrers under <strong>Application Restrictions</strong>. This allows you to restrict your key to just your site(s) for extra security. <strong>This is very important or someone could steal your key and potentially abuse it, resulting in charges to your account!&nbsp;<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5dc0c06504286364bc9154e9/file-qfLjTKBjha.png" /></strong>
    </li>
    <li>If you choose to restrict the APIs your key can access, be sure to include Places API, Maps JavaScript API, and&nbsp;Geocoding API.&nbsp;
    </li>
    <li>Once you have done the above, you should be good to go! Just add it to your settings under Settings &gt; CheckoutWC &gt; General &gt; Google API Key.&nbsp;
    </li>
  </ol>
  <h2>
    Troubleshooting
  </h2>
  <ol>
    <li>If you see exclamation points in the address field, open your browser's dev console. You will see an error message from Google indicating the problem preventing the APIs from loading.
    </li>
    <li>The most common mistake is failing to enable the required APIs (Maps, Places, Geocoding) on both the Project and the API Key itself.
    </li>
  </ol>
