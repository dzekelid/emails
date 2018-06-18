---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "9582"
tags: Emails
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid Delete Suppression Inval Emails
  x-api-slug: sendgrid
  description: "**This endpoint allows you to remove email addresses from your invalid
    email address list.**\n\nThere are two options for deleting invalid email addresses:
    \n\n1) You can delete all invalid email addresses by setting `delete_all` to true
    in the request body.\n2) You can delete some invalid email addresses by specifying
    certain addresses in an array in the request body.\n\nAn invalid email occurs
    when you attempt to send email to an address that is formatted in a manner that
    does not meet internet email format standards or the email does not exist at the
    recipient\u2019s mail server.\n\nExamples include addresses without the \u201C@\u201D
    sign or addresses that include certain special characters and/or spaces. This
    response can come from our own server or the recipient mail server.\n\nFor more
    information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/invalid_emails
  tags: Email,Suppression, Inval, Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/sendgrid/suppressioninvalid-emails-delete-openapi.md
- name: SendGrid Get Suppression Inval Emails
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a list of all invalid email
    addresses.**\n\nAn invalid email occurs when you attempt to send email to an address
    that is formatted in a manner that does not meet internet email format standards
    or the email does not exist at the recipient\u2019s mail server.\n\nExamples include
    addresses without the \u201C@\u201D sign or addresses that include certain special
    characters and/or spaces. This response can come from our own server or the recipient
    mail server.\n\nFor more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/invalid_emails
  tags: Email,Suppression, Inval, Emails
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/sendgrid/suppressioninvalid-emails-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/sendgrid/suppressioninvalid-emails-get-openapi.md
- name: SendGrid Delete Suppression Inval Emails Email
  x-api-slug: sendgrid
  description: "**This endpoint allows you to remove a specific email address from
    the invalid email address list.**\n\nAn invalid email occurs when you attempt
    to send email to an address that is formatted in a manner that does not meet internet
    email format standards or the email does not exist at the recipient\u2019s mail
    server.\n\nExamples include addresses without the \u201C@\u201D sign or addresses
    that include certain special characters and/or spaces. This response can come
    from our own server or the recipient mail server.\n\nFor more information, please
    see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/invalid_emails/{email}
  tags: Email,Suppression, Inval, Emails, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/sendgrid/suppressioninvalid-emailsemail-delete-openapi.md
- name: SendGrid Get Suppression Inval Emails Email
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a specific invalid email addresses.**\n\nAn
    invalid email occurs when you attempt to send email to an address that is formatted
    in a manner that does not meet internet email format standards or the email does
    not exist at the recipient\u2019s mail server.\n\nExamples include addresses without
    the \u201C@\u201D sign or addresses that include certain special characters and/or
    spaces. This response can come from our own server or the recipient mail server.\n\nFor
    more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/invalid_emails/{email}
  tags: Email,Suppression, Inval, Emails, Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/sendgrid/suppressioninvalid-emailsemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/sendgrid/suppressioninvalid-emailsemail-get-openapi.md
- name: SendGrid
  x-api-slug: sendgrid
  description: SendGrids cloud-based email infrastructure relieves businesses of the
    cost and complexity of maintaining custom email systems. SendGrid provides reliable
    delivery, scalability and real-time analytics along with flexible APIs that make
    custom integration a breeze.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/sendgrid/openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---