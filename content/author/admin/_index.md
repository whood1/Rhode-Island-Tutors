+++
# Display name
name = "Rhode Island Tutors"

# Username (this should match the folder name)
authors = ["admin"]

# Is this the primary user of the site?
superuser = true

# Role/position
role = "Personalized Tutoring and Test Prep"

# Organizations/Affiliations
#   Separate multiple entries with a comma, using the form: `[ {name="Org1", url=""}, {name="Org2", url=""} ]`.
#organizations = [ { name = "", url = "" } ]

# Short bio (displayed in user profile at end of posts)
bio = ""

# Enter email to display Gravatar (if Gravatar enabled in Config)
email = ""

# List (academic) interests or hobbies
#interests = [
#  "Artificial Intelligence",
#  "Computational Linguistics",
#  "Information Retrieval"
#]

# Organizational groups that you belong to (for People widget)
#   Set this to `[]` or comment out if you are not using People widget.
#user_groups = ["Researchers", "Visitors"]

# List qualifications (such as academic degrees)
#[[education.courses]]
#  course = "Tutoring"
#  institution = "Stanford University"
# year = 2019

#[[education.courses]]
#  course = "Ap Tutoring"
# institution = "Massachusetts Institute of Technology"
# year = 2019

#[[education.courses]]
# course = "SAT/ACT Test Prep"
# institution = "Massachusetts Institute of Technology"
# year = 2019

# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/widgets/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.

[[social]]
  icon = "envelope"
  icon_pack = "fas"
  link = "#contact"  # For a direct email link, use "mailto:test@example.org".

[[social]]
  icon = "twitter"
  icon_pack = "fab"
  link = "https://twitter.com/GeorgeCushen"

#[[social]]
#  icon = "google-scholar"
#  icon_pack = "ai"
#  link = "https://scholar.google.co.uk/citations?user=sIwtMXoAAAAJ"

#[[social]]
#  icon = "github"
#  icon_pack = "fab"
#  link = "https://github.com/gcushen"

# Link to a PDF of your resume/CV from the About widget.
# To enable, copy your resume/CV to `static/files/cv.pdf` and uncomment the lines below.
# [[social]]
#   icon = "cv"
#   icon_pack = "ai"
#   link = "files/cv.pdf"

+++

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.2/jquery.min.js"></script>

<script src="https://cdn.snipcart.com/scripts/2.0/snipcart.js" data-api-key="MzM0YmExMzAtYmUxYi00MGYxLTkwNmUtOWNiN2ZmNjMyMjYwNjM2OTQ1MDMzNDI1ODkyMDE4" id="snipcart"></script>

<link rel="stylesheet" href="base/snipcart.css" type="text/css" />

<!-- Load Stripe.js on your website. -->
<script src="https://js.stripe.com/v3"></script>

<!-- Create a button that your customers click to complete their purchase. Customize the styling to suit your branding. -->
<button
  style="background-color:#6772E5;color:#FFF;padding:8px 12px;border:0;border-radius:4px;font-size:1em"
  id="checkout-button-sku_F8knIfXxwcOhAv"
  role="link"
>
  Purchase Hour
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


**Rhode Island Tutors** is based out of southern Rhode Island and offers high quality summer tutoring and test preparation services. 

Whether your student is a achieving senior that wants an edge for their college applications or a freshman that just wants to sharpen their skills and build a solid foundation for continuing education, we offer personalized, 1:1 tutoring that can cater to any educational needs.

Please scroll down to see more about us & our services, and feel free 
to contact us with any questions.

[Test](/static/onehour.html")

<button
    class="snipcart-add-item"
    data-item-id="1"
    data-item-name="One Hour Session"
    data-item-price="25.00"
    data-item-weight="1"
    data-item-url="http://ritutoring.com"
    data-item-description="One hour long personalized tutoring session.">
        Purchase Session
</button>

