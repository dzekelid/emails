---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Put Gigme Email Save
  version: 1.0.0
  description: Put gigme email save.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/email/send:
    post:
      summary: Post Email Send
      description: Post email send.
      operationId: postApiV1EmailSend
      x-api-path-slug: apiv1emailsend-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Send
  /api/v1/email/confirm:
    post:
      summary: Post Email Confirm
      description: Post email confirm.
      operationId: postApiV1EmailConfirm
      x-api-path-slug: apiv1emailconfirm-post
      parameters:
      - in: body
        name: request
        description: email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Confirm
  /api/v1/email/save:
    put:
      summary: Put Email Save
      description: Put email save.
      operationId: putApiV1EmailSave
      x-api-path-slug: apiv1emailsave-put
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: email
        description: Email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Save
  /api/v1/gigme/email/save:
    put:
      summary: Put Gigme Email Save
      description: Put gigme email save.
      operationId: putApiV1GigmeEmailSave
      x-api-path-slug: apiv1gigmeemailsave-put
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: email
        description: Email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Email
      - Save
  /api/v1/gigme/email/send:
    post:
      summary: Post Gigme Email Send
      description: Post gigme email send.
      operationId: postApiV1GigmeEmailSend
      x-api-path-slug: apiv1gigmeemailsend-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Email
      - Send
  /api/v1/gigme/email/confirm:
    post:
      summary: Post Gigme Email Confirm
      description: Post gigme email confirm.
      operationId: postApiV1GigmeEmailConfirm
      x-api-path-slug: apiv1gigmeemailconfirm-post
      parameters:
      - in: body
        name: request
        description: email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Email
      - Confirm
  /api/v1/admin/user/emailAndPhone/{userId}:
    post:
      summary: Post Admin User Emailandphone Userid
      description: Post admin user emailandphone userid.
      operationId: postApiV1AdminUserEmailandphoneUser
      x-api-path-slug: apiv1adminuseremailandphoneuserid-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Emailandphone
      - Userid
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