---
swagger: "2.0"
x-collection-name: NPR
x-complete: 0
info:
  title: NPR Send a donation email to the logged-in user (only on request)
  description: This will send a station-specific donation email to the logged-in user.
  termsOfService: http://dev.npr.org/develop/terms-of-use
  contact:
    name: NPR One Enterprise Team
    url: http://dev.npr.org
    email: NPROneEnterprise@npr.org
  version: 1.0.0
host: api.npr.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /localactivation/v2/donate_email:
    get:
      summary: Send a donation email to the logged-in user (only on request)
      description: This will send a station-specific donation email to the logged-in
        user.
      operationId: sendDonationEmail
      x-api-path-slug: localactivationv2donate-email-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - News
      - Localactivation
      - Donate
      - Email
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