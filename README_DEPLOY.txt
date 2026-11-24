STEFANIA BELLINI WEBSITE: HOW TO PUBLISH (GitHub Pages)

WHAT IS IN THIS FOLDER (upload ALL of it, including the img folder)
  index.html        the whole website
  img/              the pictures of the website (18 files)
  og-image.jpg      the preview picture shown when the link is shared
  CNAME             the web address: stefaniabellini.it
  robots.txt        tells search engines they may read the site
  sitemap.xml       the list of pages for Google
  404.html          the "page not found" page
  .nojekyll         optional; GitHub works without it, so do not worry if your computer hides it

1. UPLOAD
   Unzip the folder on the computer first. In the GitHub repository click "Add file", then "Upload files",
   and drag in the CONTENTS of the folder (index.html, img, og-image.jpg, CNAME, robots.txt, sitemap.xml, 404.html).
   The img folder must keep its name. Click "Commit changes".

2. PUBLISH
   Settings, then Pages. Source: "Deploy from a branch". Branch: main, folder: / (root). Save.
   Custom domain: stefaniabellini.it. Save. When it is available, tick "Enforce HTTPS".

3. DNS (at Aruba)
   Four A records for the main address:
   185.199.108.153   185.199.109.153   185.199.110.153   185.199.111.153
   One CNAME record: name www, value stefaniabelliniw-cyber.github.io
   Delete older A or CNAME records for the same names. Do not touch MX or TXT records (email).
   It can take a few minutes to some hours. Always check GitHub's current documentation, because values can change.

4. CONTACT FORM
   The form now opens an email for the visitor to send. For messages to arrive by themselves, use a form service
   such as Web3Forms: register with the mailbox address, copy the access key from the email, then in index.html
   find  var FORM={endpoint:"",extra:{}};  and set the endpoint given by the service and extra to {access_key:"KEY"}.
   Test with a real message.

5. GOOGLE (so the site can be found)
   a. Go to search.google.com/search-console and sign in with stefania.bellini.w@gmail.com.
   b. Add the property. The easiest way is "URL prefix": https://stefaniabellini.it/ and the verification
      with an HTML file: download the file Google gives you and upload it to the repository, next to index.html.
      Then click Verify.
   c. In "Sitemaps", enter sitemap.xml and submit.
   d. In the URL inspection bar at the top, paste https://stefaniabellini.it/ and click "Request indexing".
   e. Claim the free Google Business or knowledge profile only if it applies. Link the site from Facebook, Instagram,
      LinkedIn, X, Amazon author page, Goodreads, Europe Books and every press page that mentions her.

6. TEST BEFORE ANNOUNCING
   Every menu item and button, on a phone and on a computer; the PayPal link with a small real payment;
   the shop and press links; the contact form with a real message; the address with https:// and with www.
