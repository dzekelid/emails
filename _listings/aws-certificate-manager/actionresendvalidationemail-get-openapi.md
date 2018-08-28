---
swagger: "2.0"
x-collection-name: AWS Certificate Manager
x-complete: 0
info:
  title: AWS Certificate Manager API Resend Validation Email
  version: 1.0.0
  description: Resends the email that requests domain ownership validation.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResendValidationEmail:
    get:
      summary: Resend Validation Email
      description: Resends the email that requests domain ownership validation.
      operationId: ResendValidationEmail
      x-api-path-slug: actionresendvalidationemail-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains the ARN of the requested certificate
        type: string
      - in: query
        name: Domain
        description: The Fully Qualified Domain Name (FQDN) of the certificate that
          needs to be      validated
        type: string
      - in: query
        name: ValidationDomain
        description: The base validation domain that will act as the suffix of the
          email addresses that are      used to send the emails
        type: string
      responses:
        200:
          description: OK
      tags:
      - Validation Email
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