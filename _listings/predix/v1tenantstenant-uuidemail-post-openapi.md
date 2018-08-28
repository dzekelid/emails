---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Notification Service Post Tenants Email
  description: Post tenants email.
  version: 1.0.0
host: ev-notification-service.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/tenants/{tenant_uuid}/email:
    post:
      summary: Post Tenants Email
      description: Post tenants email.
      operationId: postV1TenantsTenantUuEmail
      x-api-path-slug: v1tenantstenant-uuidemail-post
      parameters:
      - in: body
        name: applicationMessage
        description: applicationMessage
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: configuration
        description: configuration
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Email
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