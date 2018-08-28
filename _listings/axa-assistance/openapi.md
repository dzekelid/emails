swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 1
info:
  title: AXA Assistance
  description: axa-assistance-is-a-worldwide-specialist-for-car-insurance-travel-health-and-home-services--trust-in-axa-assistance-for-your-insurance
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