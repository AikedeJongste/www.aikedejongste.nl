---
layout: post
title:  "What you need to know about SSL certificates"
date:   2018-01-15 13:37 +0200
categories: need-to-know
---

If you have a website or a web application you must have heard about
certificates for your website/application. They are often called
SSL certificates. Most of the time you hear about them when they are expired or
when the registrar starts sending you email reminders to extend the certificate.

SSL-certificates are important. Every website and application should have one.
Here is why:

1. They guarantee that the website the user receives and sees is the same as the
   one you have on your server or webhosting account and nobody could intercept
   the connection. That’s why online banking sites were the first to use
   SSL certificates. They don’t want passwords and bank statements leaking while
   they are being transmitted to the user.
2. Another party that may change the information being transmitted is the
   internet provider. In some countries (especially Indonesia) they insert
   visible advertisements into websites. In other countries it’s often invisible
   trackers. When you serve your website over https with a SSL certificate this
   is not possible.  Passwords stay secret and no advertisements will be injected.
3. Search engines are pushing towards a fully encrypted internet where every
   site is only available over https and thus has a certificate. They do
   this by rewarding sites with a certificate with a higher position in the
   search results. So yes, a certificate is good for your SEO score.
4. Certificates can also be used to guarantee the authenticity of your website.
   If you order an EV certificate the certificate authority will do a thorough
   check to verify your company. This is also why EV (extended validation)
   certificates are more expensive. For most businesses and websites this is not
   required. Banks obviously have these certificates and you can recognize them
   by the name in the address bar in your browser.

![Different types](/assets/certificates.png){:class="img-responsive"}

What should I do, now that I know this?

1. Find out if your website or application has a certificate. Open a browser and go to
httpS://www.yourwebsite.com. If you see your website and your browser shows no
errors you’ve got one! In Google Chrome there will be a little green lock icon in
front of the url.
2. It's also important to make sure all visitors are redirected to the
   https-version of your website. This means that if they go to
   http://yourwebsite.com they are automatically redirected to
   httpS://yourwebsite.com.

**Pro-tip:** verfiy that the certificate is installed properly on the [SSL Labs
website](https://www.ssllabs.com/ssltest/). Enter your domain name and wait for
the test suite to complete. It's free and takes about 2 minutes. If the result
of the test is a B or lower you have some things you need to improve.

**Pro-tip:** setup a monitoring tool to warn you when your certificate is about
to expire. I'll explain this in another blogpost.


