---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact List Account Email Addresses
  description: List Account Email Addresses
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---