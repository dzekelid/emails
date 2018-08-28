swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizers:
    get:
      summary: Organizer by email
      description: Gets the individual organizer specified by the organizer's email
        address. If an email address is not specified, all organizers are returned.
        This API call is only available to users with the admin role.
      operationId: OrganizersGet
      x-api-path-slug: organizers-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: email
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - By
      - Email
    delete:
      summary: Organizer by email
      description: Deletes the individual organizer specified by the email address.
        This API call is only available to users with the admin role.
      operationId: OrganizersDelete
      x-api-path-slug: organizers-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: email
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - By
      - Email