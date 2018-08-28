swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
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