+++
# Experience widget.
widget = "experience"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 3  # Order that this section will appear.

title = "Services"
subtitle = ""

# Date format for experience
#   Refer to https://sourcethemes.com/academic/docs/customization/#date-format
date_format = ""

# Experiences.
#   Add/remove as many `[[experience]]` blocks below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin/end multi-line descriptions with 3 quotes `"""`.
[[experience]]
  title = "Tutoring"
  company = "25$/hr"
  company_url = ""
  location = ""
  date_start = "2016-01-01"
  date_end = ""
  description = """
  Personalized tutoring.
  (Inquire about tutoring for AP-level classes. No tutoring for foriegn languages offered at this time.)
  <!-- Load Stripe.js on your website. -->
<script src="https://js.stripe.com/v3"></script>

<!-- Create a button that your customers click to complete their purchase. Customize the styling to suit your branding. -->
<button
  style="background-color:#24C2CB;color:#FFF;padding:8px 12px;border:0;border-radius:4px;font-size:1em"
  id="checkout-button-sku_F8knIfXxwcOhAv"
  role="link"
>
  Purchase Hour Session
</button>

<div id="error-message"></div>

<script>
  var stripe = Stripe('pk_live_5yTvLS4dlrxxxeRnIxGYM5nT00LmGskNHp');

  var checkoutButton = document.getElementById('checkout-button-sku_F8knIfXxwcOhAv');
  checkoutButton.addEventListener('click', function () {
    // When the customer clicks on the button, redirect
    // them to Checkout.
    stripe.redirectToCheckout({
      items: [{sku: 'sku_F8knIfXxwcOhAv', quantity: 1}],

      // Do not rely on the redirect to the successUrl for fulfilling
      // purchases, customers may not always reach the success_url after
      // a successful payment.
      // Instead use one of the strategies described in
      // https://stripe.com/docs/payments/checkout/fulfillment
      successUrl: window.location.protocol + '//ritutoring.com/success',
      cancelUrl: window.location.protocol + '//ritutoring.com/canceled',
    })
    .then(function (result) {
      if (result.error) {
        // If `redirectToCheckout` fails due to a browser or network
        // error, display the localized error message to your customer.
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
</script>

    """

#[[experience]]
#  title = "AP Tutoring"
#  company = "30$/hr"
# company_url = ""
#  date_start = "2016-01-01"
# date_end = ""
# description = """
#  AP Chemistry, Literature, Calculus, US History, Psychology or #quivalent.
# 
# """



[[experience]]
 title = "SAT/ACT Test Prep"
 company = "30$/hr"
 company_url = ""
 location = ""
 date_start = "2016-01-01"
 date_end = ""
 description = """
 Personalized test preparation for the SAT or ACT Test.
 (No preparation for SAT Subject Tests offered at this time.)
 
 <!-- Load Stripe.js on your website. -->
<script src="https://js.stripe.com/v3"></script>

<!-- Create a button that your customers click to complete their purchase. Customize the styling to suit your branding. -->
<button
  style="background-color:#24C2CB;color:#FFF;padding:8px 12px;border:0;border-radius:4px;font-size:1em"
  id="checkout-button-sku_FA1DHFTCTGqdoz"
  role="link"
>
  Purchase Hour Session
</button>

<div id="error-message"></div>

<script>
  var stripe = Stripe('pk_live_5yTvLS4dlrxxxeRnIxGYM5nT00LmGskNHp');

  var checkoutButton = document.getElementById('checkout-button-sku_FA1DHFTCTGqdoz');
  checkoutButton.addEventListener('click', function () {
    // When the customer clicks on the button, redirect
    // them to Checkout.
    stripe.redirectToCheckout({
      items: [{sku: 'sku_FA1DHFTCTGqdoz', quantity: 1}],

      // Do not rely on the redirect to the successUrl for fulfilling
      // purchases, customers may not always reach the success_url after
      // a successful payment.
      // Instead use one of the strategies described in
      // https://stripe.com/docs/payments/checkout/fulfillment
      successUrl: window.location.protocol + '//ritutoring.com/success',
      cancelUrl: window.location.protocol + '//ritutoring.com/canceled',
    })
    .then(function (result) {
      if (result.error) {
        // If `redirectToCheckout` fails due to a browser or network
        // error, display the localized error message to your customer.
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
</script>
 
 """

+++
