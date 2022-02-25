---
title: Common Problems and Solutions
slug: common-problems-and-solutions
cats: Troubleshooting
---

Error: Account username is a required field. 
---------------------------------------------

 This means WooCommerce is not configured to automatically generate a username. You can change this by going to WooCommerce -&gt; Settings -&gt; Accounts &amp; Privacy:

 ![](https://s3.amazonaws.com/helpscout.net/docs/assets/5bdde2822c7d3a01757ac42e/images/5c69b6df042863543ccd18e8/file-55oqqTFoVc.png)

Error: We were unable to process your order, please try again.
--------------------------------------------------------------

 This indicates that WooCommerce is unable to verify the nonce it uses to verify checkout submits are authentic.

 This usually means you are running an old version of WooCommerce (&lt;3.4). To fix this, update to the latest version of WooCommerce.

Error: Could not connect to server. Please refresh and try again or contact site administrator.
-----------------------------------------------------------------------------------------------

 User browser is unable to connect to server.

Error: Requested resource could not be found. Please contact site administrator. (404)
--------------------------------------------------------------------------------------

AJAX end point returned a 404 error. This usually indicates a server issue.

Error: An internal server error occurred. Please contact site administrator. (500) 
-----------------------------------------------------------------------------------

 Server returned 500 error. Usually a PHP fatal error which can be viewed in your error logs.

Error: Server response could not be parsed. Please contact site administrator.
------------------------------------------------------------------------------

 Server did not return JSON formatted response.

Error: The server timed out while processing your request. Please refresh and try again or contact site administrator.
----------------------------------------------------------------------------------------------------------------------

 Server returned 504 error or otherwise timed out. This is usually a server side performance problem unrelated to CheckoutWC.

Error: Request was aborted. Please contact site administrator.
--------------------------------------------------------------

 AJAX request was aborted. This would generally only happen in the unusual event a user used their browser's dev tools to cancel an AJAX request, but it may also happen if the server disconnects during a response.

Error: Uncaught Error: &lt;error message&gt;
--------------------------------------------

 Returned if the server returns an error condtion not anticipated in the previous error checks.