swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{USER_ID}/email_aliases:
    get:
      summary: Get Email Aliases
      description: Retrieves all email aliases for this user. The collection of email
        aliases does not include the primary login for the user; use GET /users/USER_ID
        to retrieve the login email address.
      operationId: getEmailAliases
      x-api-path-slug: usersuser-idemail-aliases-get
      parameters:
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
      - ""
      - Email
      - Aliases
    post:
      summary: Add Email Alias
      description: Adds a new email alias to the given user???s account.
      operationId: addEmailAlias
      x-api-path-slug: usersuser-idemail-aliases-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
      - ""
      - Email
      - Aliases
  /users/{USER_ID}/email_aliases/{EMAIL_ALIAS_ID}:
    delete:
      summary: Delete Email Alias
      description: Removes an email alias from a user.
      operationId: deleteUserEmailAlias
      x-api-path-slug: usersuser-idemail-aliasesemail-alias-id-delete
      parameters:
      - in: path
        name: EMAIL_ALIAS_ID
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
      - ""
      - Email
      - Aliases
      - Email
      - Alias