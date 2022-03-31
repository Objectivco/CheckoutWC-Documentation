---
title: How to Install CheckoutWC With Composer
slug: how-to-install-checkoutwc-with-composer
cats: How To
---

<p>If you're a developer who loves managing dependencies with Composer (we certainly do) you can install CheckoutWC with composer. Here are the steps!</p>
<h2>Add Our Repository</h2>
<pre><code>{
	&quot;repositories&quot;: [
		{
			&quot;type&quot;: &quot;composer&quot;,
			&quot;url&quot;: &quot;https://www.checkoutwc.com/composer/{YourLicenseKey}&quot;
		}
	]
}
</code></pre>
<p>Substitute {YourLicenseKey} with your actual license key.</p>
<h2>Add Our Plugin</h2>
<p>From your CLI (terminal) run: ```
composer require objectivco/checkout-for-woocommerce</p>
<pre><code>
Version Constraints
-------------------

 You can use any [Composer version constraints](https://getcomposer.org/doc/articles/versions.md), or specify the exact version of a plugin or addon:

</code></pre>
<p>&quot;require&quot;: {
&quot;objectivco/checkout-for-woocommerce&quot;: &quot;3.7.1&quot;
}</p>
<pre><code>
Example composer.json
---------------------

</code></pre>
<p>{
&quot;name&quot;: &quot;your/project&quot;,
&quot;description&quot;: &quot;A CheckoutWC site&quot;,
&quot;repositories&quot;: [
{
&quot;type&quot;: &quot;composer&quot;,
&quot;url&quot;: &quot;https://www.checkoutwc.com/composer/123456890&quot;
}
],
&quot;require&quot;: {
&quot;objectivco/checkout-for-woocommerce&quot;: &quot;^3.7&quot;
}
}</p>
<pre><code></code></pre>
