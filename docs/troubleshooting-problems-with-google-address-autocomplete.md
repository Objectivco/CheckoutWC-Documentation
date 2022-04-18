---
title: Troubleshooting Problems with Google Address Autocomplete
slug: troubleshooting-problems-with-google-address-autocomplete
cats: Troubleshooting
---


  <p>
    If there's a problem with your Google API key you will see something like this on your checkout page:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6202a5dad86136157d9a20d3/file-oDNJ7yjouK.png" />
  </p>
  <p>
    This indicates that there's a problem with your Google API Key. This isn't a CheckoutWC issue.&nbsp;
  </p>
  <p>
    To determine what the problem is, <a href="https://cfw.staging.objectiv.co/documentation/how-to-access-your-browsers-developer-tools-for-debugging" target="_blank">open up your browser's developer tools</a> and check the console for a log entry like this:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/6202a73b68cd260cc2d38faf/file-APMTqS5on6.png" />
  </p>
  <h2>
    Most common problems:
  </h2>
  <ol>
    <li>The API key is not allowed on the current site. (RefererNotAllowedMapError)
    </li>
    <li>The API key doesn't have access to the necessary APIs. (Maps, Places, Geocoding)
    </li>
    <li>The project doesn't have access to the necessary APIs (Maps, Places, Geocoding)
    </li>
    <li>Your Google Cloud Project doesn't have billing enabled.
    </li>
  </ol>
