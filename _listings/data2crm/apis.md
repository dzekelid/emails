---
name: Data2CRM
x-slug: data2crm
description: Data2CRM is all-in-one master touch instrument to create the perfect
  data environment for prosperous internal and external connections.Data2CRM.API,
  a Unified API Provider, to Connect Your Business Software with 17+ CRMs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Emails
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/apis.md
specificationVersion: "0.14"
apis:
- name: Data2CRM GET for Email
  x-api-slug: data2crm
  description: Returns all emails from the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//email
  tags: Emails
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/email-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/email-get-openapi.md
- name: Data2CRM POST for Email
  x-api-slug: data2crm
  description: Add email into the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//email
  tags: Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/email-post-openapi.md
- name: Data2CRM COUNT for Email
  x-api-slug: data2crm
  description: Count all emails from the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//email/count
  tags: Emails,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/emailcount-get-openapi.md
- name: Data2CRM DESCRIBE for Email
  x-api-slug: data2crm
  description: Returns describe for emails
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//email/describe
  tags: Emails,Describe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/emaildescribe-get-openapi.md
- name: Data2CRM DELETE for Email
  x-api-slug: data2crm
  description: Delete email information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//email/{email_id}
  tags: Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/emailemail-id-delete-openapi.md
- name: Data2CRM GET for Email
  x-api-slug: data2crm
  description: Return email information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//email/{email_id}
  tags: Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/emailemail-id-get-openapi.md
- name: Data2CRM PUT for Email
  x-api-slug: data2crm
  description: Update email information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//email/{email_id}
  tags: Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/emailemail-id-put-openapi.md
- name: Data2CRM
  x-api-slug: data2crm
  description: Data2CRM is all-in-one master touch instrument to create the perfect
    data environment for prosperous internal and external connections.Data2CRM.API,
    a Unified API Provider, to Connect Your Business Software with 17+ CRMs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1
  tags: Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/data2crm/openapi.md
x-common:
- type: x-twitter
  url: https://twitter.com/data2crm
- type: x-website
  url: http://data2crm.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---