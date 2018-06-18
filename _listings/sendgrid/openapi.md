---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  description: the-sendgrid-web-api-v3-documentation--this-is-the-entirety-of-the-documented-v3-endpoints--we-have-updated-all-the-descriptions-parameters-requests-and-responses--authentication-every-endpoint-requires-authentication-in-the-form-of-an-authorization-header-authorization-bearer-api-key
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /suppression/invalid_emails:
    delete:
      summary: Delete Suppression Inval Emails
      description: "**This endpoint allows you to remove email addresses from your
        invalid email address list.**\n\nThere are two options for deleting invalid
        email addresses: \n\n1) You can delete all invalid email addresses by setting
        `delete_all` to true in the request body.\n2) You can delete some invalid
        email addresses by specifying certain addresses in an array in the request
        body.\n\nAn invalid email occurs when you attempt to send email to an address
        that is formatted in a manner that does not meet internet email format standards
        or the email does not exist at the recipient\u2019s mail server.\n\nExamples
        include addresses without the \u201C@\u201D sign or addresses that include
        certain special characters and/or spaces. This response can come from our
        own server or the recipient mail server.\n\nFor more information, please see
        our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
      operationId: suppression.invalid_emails.delete
      x-api-path-slug: suppressioninvalid-emails-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Suppression
      - Inval
      - Emails
    get:
      summary: Get Suppression Inval Emails
      description: "**This endpoint allows you to retrieve a list of all invalid email
        addresses.**\n\nAn invalid email occurs when you attempt to send email to
        an address that is formatted in a manner that does not meet internet email
        format standards or the email does not exist at the recipient\u2019s mail
        server.\n\nExamples include addresses without the \u201C@\u201D sign or addresses
        that include certain special characters and/or spaces. This response can come
        from our own server or the recipient mail server.\n\nFor more information,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
      operationId: suppression.invalid_emails.get
      x-api-path-slug: suppressioninvalid-emails-get
      parameters:
      - in: query
        name: end_time
        description: Refers end of the time range in unix timestamp when an invalid
          email was created (inclusive)
      - in: query
        name: limit
        description: Limit the number of results to be displayed per page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: Paging offset
      - in: query
        name: start_time
        description: Refers start of the time range in unix timestamp when an invalid
          email was created (inclusive)
      responses:
        200:
          description: OK
      tags:
      - Email
      - Suppression
      - Inval
      - Emails
  /suppression/invalid_emails/{email}:
    delete:
      summary: Delete Suppression Inval Emails Email
      description: "**This endpoint allows you to remove a specific email address
        from the invalid email address list.**\n\nAn invalid email occurs when you
        attempt to send email to an address that is formatted in a manner that does
        not meet internet email format standards or the email does not exist at the
        recipient\u2019s mail server.\n\nExamples include addresses without the \u201C@\u201D
        sign or addresses that include certain special characters and/or spaces. This
        response can come from our own server or the recipient mail server.\n\nFor
        more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
      operationId: suppression.invalid_emails.email.delete
      x-api-path-slug: suppressioninvalid-emailsemail-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Suppression
      - Inval
      - Emails
      - Email
    get:
      summary: Get Suppression Inval Emails Email
      description: "**This endpoint allows you to retrieve a specific invalid email
        addresses.**\n\nAn invalid email occurs when you attempt to send email to
        an address that is formatted in a manner that does not meet internet email
        format standards or the email does not exist at the recipient\u2019s mail
        server.\n\nExamples include addresses without the \u201C@\u201D sign or addresses
        that include certain special characters and/or spaces. This response can come
        from our own server or the recipient mail server.\n\nFor more information,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
      operationId: suppression.invalid_emails.email.get
      x-api-path-slug: suppressioninvalid-emailsemail-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Suppression
      - Inval
      - Emails
      - Email
---