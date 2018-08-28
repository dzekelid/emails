---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Resends the confirmation email to an identity account
  description: Resends the confirmation email to an identity account
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/v1/identities/register/confirm/resend:
    post:
      summary: Resends the confirmation email to an identity account
      description: Resends the confirmation email to an identity account
      operationId: postUserV1IdentitiesRegisterConfirmResend
      x-api-path-slug: userv1identitiesregisterconfirmresend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - ResendAssistance
      - the
      - confirmation
      - email
      - toidentity
      - account
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