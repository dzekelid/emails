---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 1
info:
  title: Bitbucket
  description: code-against-the-bitbucket-api-to-automate-simple-tasks-embed-bitbucket-data-into-your-own-site-build-mobile-or-desktop-apps-or-even-add-custom-ui-addons-into-bitbucket-itself-using-the-connect-framework-
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/emails:
    get:
      summary: Get User Emails
      description: |-
        Returns all the authenticated user's email addresses. Both
        confirmed and unconfirmed.
      operationId: getUserEmails
      x-api-path-slug: useremails-get
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
    parameters:
      summary: Parameters User Emails
      description: Parameters user emails
      operationId: parametersUserEmails
      x-api-path-slug: useremails-parameters
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
  /user/emails/{email}:
    get:
      summary: Get User Emails Email
      description: |-
        Returns details about a specific one of the authenticated user's
        email addresses.

        Details describe whether the address has been confirmed by the user and
        whether it is the user's primary address or not.
      operationId: getUserEmailsEmail
      x-api-path-slug: useremailsemail-get
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
      - Email
    parameters:
      summary: Parameters User Emails Email
      description: Parameters user emails email
      operationId: parametersUserEmailsEmail
      x-api-path-slug: useremailsemail-parameters
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
      - Email
---