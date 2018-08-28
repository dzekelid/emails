---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Gets user data by email
  version: 1.0.0
  description: Gets user data by email.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/by-email/{email}:
    get:
      summary: Gets user data by email
      description: Gets user data by email.
      operationId: getUserByEmail
      x-api-path-slug: usersbyemailemail-get
      parameters:
      - in: path
        name: email
      responses:
        200:
          description: OK
      tags:
      - User
      - Data
      - By
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