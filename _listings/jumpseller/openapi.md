swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 1
info:
  title: Jumpseller
  description: explore-all-our-endpoints-with-your-own-set-of-of-access-tokens--all-changes-affect-your-production-jumpseller-store-
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers/email/{email}.json:
    get:
      summary: Get Customers Email Email
      description: Retrieve a single customer..
      operationId: getCustomersEmailEmail.json
      x-api-path-slug: customersemailemail-json-get
      parameters:
      - in: path
        name: email
        description: Email of the Customer
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Email
      - Email
      - Json