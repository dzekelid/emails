---
swagger: "2.0"
x-collection-name: Mynewsdesk
x-complete: 0
info:
  title: My News Desk Pressroom List Send Email
  description: Send Email
  termsOfService: http://www.mynewsdesk.com/about/terms-and-conditions?locale=en
  version: v1
host: www.mynewsdesk.com
basePath: /services/pressroom/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  send_email/:
    get:
      summary: Send Email
      description: Send Email
      operationId: getSendEmail
      x-api-path-slug: send-email-get
      parameters:
      - in: query
        name: from
        description: Name of sender
      - in: query
        name: item_id
        description: ID of the material to be fetched
      - in: query
        name: message
        description: Personal message from the sender to the recipient
      - in: query
        name: to_email
        description: Recipient email address
      - in: query
        name: type_of_media
        description: The type of material to be fetched
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - Send
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