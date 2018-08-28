swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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