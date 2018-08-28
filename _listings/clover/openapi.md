swagger: "2.0"
x-collection-name: Clover
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/customers/{customerId}/email_addresses:
    post:
      summary: Create an email address for a customer
      description: Creates an email address associated to a merchant's customer.
      operationId: DelegatedCreateCustomerEmailAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridemail-addresses-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Email
      - Addresses
  /v3/merchants/{mId}/customers/{customerId}/email_addresses/{emailId}:
    post:
      summary: Update an email address for a customer
      description: Updates a merchant's customer's email address.
      operationId: DelegatedUpdateCustomerEmailAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridemail-addressesemailid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: emailId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Email
      - Addresses
      - EmailId
    delete:
      summary: Delete a customer email address
      description: Deletes a merchant's customer's email address.
      operationId: DelegatedDeleteCustomerEmailAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridemail-addressesemailid-delete
      parameters:
      - in: path
        name: customerId
      - in: path
        name: emailId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Email
      - Addresses
      - EmailId