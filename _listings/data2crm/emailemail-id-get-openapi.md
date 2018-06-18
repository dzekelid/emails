---
swagger: "2.0"
x-collection-name: Data2CRM
x-complete: 0
info:
  title: Data2CRM GET for Email
  description: Return email information
  version: "1"
host: api.data2crm.com:80
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /email:
    get:
      summary: GET for Email
      description: Returns all emails from the system
      operationId: getEmailCollection
      x-api-path-slug: email-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
    post:
      summary: POST for Email
      description: Add email into the system
      operationId: createEmailEntity
      x-api-path-slug: email-post
      parameters:
      - in: body
        name: body
        description: Add email into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
  /email/count:
    get:
      summary: COUNT for Email
      description: Count all emails from the system
      operationId: getEmailCountCollection
      x-api-path-slug: emailcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
      - Count
  /email/describe:
    get:
      summary: DESCRIBE for Email
      description: Returns describe for emails
      operationId: getEmailDescribe
      x-api-path-slug: emaildescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
      - Describe
  /email/{email_id}:
    delete:
      summary: DELETE for Email
      description: Delete email information
      operationId: deleteEmailEntity
      x-api-path-slug: emailemail-id-delete
      parameters:
      - in: path
        name: email_id
        description: Email Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
    get:
      summary: GET for Email
      description: Return email information
      operationId: getEmailEntity
      x-api-path-slug: emailemail-id-get
      parameters:
      - in: path
        name: email_id
        description: Email Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
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