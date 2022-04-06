---
title: Common Problems and Solutions
slug: common-problems-and-solutions
cats: Troubleshooting
---


  <h2>
    Error: Account username is a required field.&nbsp;
  </h2>
  <p>
    This means WooCommerce is not configured to automatically generate a username. You can change this by going to WooCommerce -&gt; Settings -&gt; Accounts &amp; Privacy:
  </p>
  <p>
    <img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5c69b6df042863543ccd18e8/file-55oqqTFoVc.png" />
  </p>
  <h2>
    Error:&nbsp;We were unable to process your order, please try again.
  </h2>
  <p>
    This indicates that WooCommerce is unable to verify the nonce it uses to verify checkout submits are authentic.
  </p>
  <p>
    This usually means you are running an old version of WooCommerce&nbsp; (&lt;3.4). To fix this, update to the latest version of WooCommerce.
  </p>
  <h2>
    Error: Could not connect to server. Please refresh and try again or contact site administrator.
  </h2>
  <p>
    User browser is unable to connect to server.
  </p>
  <h2>
    Error: Requested resource could not be found. Please contact site administrator. (404)
  </h2>
  <p>
    AJAX end point returned a 404 error. This usually indicates a server issue.
  </p>
  <h2>
    Error: An internal server error occurred. Please contact site administrator. (500)
  </h2>
  <p>
    Server returned 500 error. Usually a PHP fatal error which can be viewed in your error logs.
  </p>
  <h2>
    Error: Server response could not be parsed. Please contact site administrator.
  </h2>
  <p>
    Server did not return JSON formatted response.
  </p>
  <h2>
    Error: The server timed out while processing your request. Please refresh and try again or contact site administrator.
  </h2>
  <p>
    Server returned 504 error or otherwise timed out. This is usually a server side performance problem unrelated to CheckoutWC.
  </p>
  <h2>
    Error: Request was aborted. Please contact site administrator.
  </h2>
  <p>
    AJAX request was aborted. This would generally only happen in the unusual event a user used their browser's dev tools to cancel an AJAX request, but it may also happen if the server disconnects during a response.
  </p>
  <h2>
    Error: Uncaught Error: &lt;error message&gt;
  </h2>
  <p>
    Returned if the server returns an error condtion not anticipated in the previous error checks.
  </p>
