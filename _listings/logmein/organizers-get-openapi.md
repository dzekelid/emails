---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToMeeting Organizer by email
  description: Gets the individual organizer specified by the organizer's email address.
    If an email address is not specified, all organizers are returned. This API call
    is only available to users with the admin role.
  version: 1.0.0
host: api.getgo.com
basePath: /G2M/rest
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