swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 1
info:
  title: ConstantContact
  description: constant-contact-inc-is-an-online-marketing-company-offering-email-marketing-social-media-marketing-online-survey-and-event-marketing-tools-primarily-to-small-businesses-nonprofit-organizations-and-membership-associations-
  termsOfService: http://www.constantcontact.com/uidocs/CCSiteOwnerAgreement.jsp
  version: 1.0.0
host: api.constantcontact.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/settings/emailaddresses:
    get:
      summary: List Account Email Addresses
      description: List Account Email Addresses
      operationId: list-account-email-addresses
      x-api-path-slug: usernamesettingsemailaddresses-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Account
      - Email
      - Resses
  /{username}/settings/emailaddresses/{email-id}:
    get:
      summary: Get Email Address Details
      description: Get Email Address Details
      operationId: get-email-address-details
      x-api-path-slug: usernamesettingsemailaddressesemailid-get
      parameters:
      - in: path
        name: email-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ress
      - Details