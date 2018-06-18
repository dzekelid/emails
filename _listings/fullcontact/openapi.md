---
swagger: "2.0"
x-collection-name: FullContact
x-complete: 1
info:
  title: FullContact Location API
  description: the-api-for-managing-fullcontact-locations
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
---