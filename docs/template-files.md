---
title: Template Files
slug: template-files
cats: Developers
---

<p>Checkout for WooCommerce has the following structure for its template files:</p>
<ul>
<li>/templates/
<ul>
<li>/template-name/
<ul>
<li>assets/</li>
<li>sources/</li>
<li>content.php</li>
<li>footer.php</li>
<li>header.php</li>
<li>screenshot.png</li>
<li>style.css</li>
<li>theme.js</li>
</ul>
</li>
</ul>
</li>
</ul>
<h2>Templates</h2>
<p><strong>checkout-for-woocommerce/templates/template-name/content.php</strong></p>
<p>This template has the bulk of the checkout page template. It's everything between the header area (essentially the title area) and the footer (copyrights).</p>
<p><strong>checkout-for-woocommerce/templates/template-name/header.php</strong></p>
<p>The header template renders the site name / logo.</p>
<p><strong>checkout-for-woocommerce/templates/template-name/footer.php</strong></p>
<p>The footer template renders the copyright information, as well as any custom text provided in settings.</p>
<h2>Folders</h2>
<p>There are two folders in the templates that ship with Checkout for WooCommerce:</p>
<h3>assets/</h3>
<p>Static assets such as images are places in this folder.</p>
<h3>sources/</h3>
<p>This folder contains the TypeScript and Sass files needed to build the template assets.</p>
<h2>Editing Templates</h2>
<p>Template files should never directly modified because they are replaced with each plugin update.</p>
<p>Instead you can over ride them in your theme. To do so, create a directory named 'checkout-wc' in your theme or child theme and copy any of the relevant templates into this directory.</p>
<p>For example, if you're using the Storefront theme with the Futurist template and you want to override the main content template file, you would copy:</p>
<p><strong>plugins/checkout-for-woocommerce/templates/futurist</strong> into <strong>themes/storefront/checkout-wc/</strong></p>
<p>And modify content.php. This is what the file structure would look like:</p>
<p><img src="https://www.checkoutwc.com/wp-content/uploads/2018/03/Screenshot-2018-11-01-10.44.37.png" alt="" /></p>
<h2>Building The Template</h2>
<p>If you want to make changes to the TypeScript or Sass files in <strong>sources/</strong>, you will need to run a few commands in terminal. We are assuming you have some basic knowledge of npm and webpack.</p>
<ol>
<li>Open terminal and cd into the template directory.</li>
<li>If this is your first time making a modification, run <strong>npm install</strong>
</li>
<li>You can then execute webpack with these commands:
<ol>
<li>
<strong>npm run dev</strong> (Builds the development versions of the TypeScript and Sass assets)</li>
<li>
<strong>npm run watch</strong> (Watches the source folder and builds the development versions of the TypeScript and Sass assets)</li>
<li>
<strong>npm run production</strong> (Builds the production versions of the TypeScript and Sass assets)</li>
</ol>
</li>
</ol>
