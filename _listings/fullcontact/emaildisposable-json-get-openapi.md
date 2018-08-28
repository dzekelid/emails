---
swagger: "2.0"
x-collection-name: FullContact
x-complete: 0
info:
  title: FullContact Lookup Email
  description: Lookup Email
  termsOfService: https://www.fullcontact.com/terms/
  version: 1.0.0
host: api.fullcontact.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /email/disposable.json:
    get:
      summary: Lookup Email
      description: Lookup Email
      operationId: lookupEmail
      x-api-path-slug: emaildisposable-json-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      - in: query
        name: email
        description: The email address that should be queried for being a disposable
          email address
      responses:
        200:
          description: OK
      tags:
      - Emails
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