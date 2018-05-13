---
swagger: "2.0"
info:
  title: Dyn Retrieve Count of Emails Sent
  version: 1.0.0
  description: Retrieve Count of Emails Sent
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  reports/sent/count:
    get:
      summary: Retrieve Count of Emails Sent
      description: Retrieve Count of Emails Sent
      operationId: getReportsSentCount
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - retrieve
      - count
      - of
      - emails
      - sent
definitions: []
x-collection-name: Dyn
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