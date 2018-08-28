---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Create a session with email and password
  description: Create a session with email and password
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /credential-hashes/emails:
    post:
      summary: Create an email credential
      description: Create an email credential
      operationId: create-an-email-credential
      x-api-path-slug: credentialhashesemails-post
      parameters:
      - in: body
        name: body
        description: Email credential resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Credential
  /credential-hashes/emails/{hash}:
    get:
      summary: Retrieve an email credential
      description: Retrieve an email credential with specified token identifier string
      operationId: retrieve-an-email-credential-with-specified-token-identifier-string
      x-api-path-slug: credentialhashesemailshash-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Email
      - Credential
  /forgot-password:
    post:
      summary: Sends an email with a link containing a token to reset user password
      description: Sends an email with a link containing a token to reset user password
      operationId: sends-an-email-with-a-link-containing-a-token-to-reset-user-password
      x-api-path-slug: forgotpassword-post
      parameters:
      - in: body
        name: body
        description: Email resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Email
      - Link
      - Containing
      - Token
      - To
      - Reset
      - User
      - Password
  /previews/rule-actions/send-email:
    post:
      summary: Send a test email
      description: Send a test email
      operationId: send-a-test-email
      x-api-path-slug: previewsruleactionssendemail-post
      parameters:
      - in: body
        name: body
        description: Test email resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Test
      - Email
  /signin:
    post:
      summary: Create a session with email and password
      description: Create a session with email and password
      operationId: create-a-session-with-email-and-password
      x-api-path-slug: signin-post
      parameters:
      - in: body
        name: body
        description: Signin resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Session
      - Email
      - Password
  /signup:
    post:
      summary: Creates a new user and sends an email confirmation
      description: Creates a new user and sends an email confirmation
      operationId: creates-a-new-user-and-sends-an-email-confirmation
      x-api-path-slug: signup-post
      parameters:
      - in: body
        name: body
        description: Signup resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - User
      - Sends
      - Email
      - Confirmation
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