---
title: Generate Password Filter
slug: generate-password-filter
cats: Developers
status: published
---


  <p>
    If WooCommerce settings allow for creating accounts while checking out we will generate a password for users who don't have an account.
  </p>
  <p>
    You can override this functionality&nbsp;in your child theme's functions.php file with the filter below.
  </p>
  <div>
    <div>
      <div>
        add_filter( 'cfw_registration_generate_password', '__return_false' );
      </div>
    </div>
  </div>
