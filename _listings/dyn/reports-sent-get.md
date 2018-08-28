---
swagger: "2.0"
info:
  title: Dyn Retrieve Emails Sent
  version: 1.0.0
  description: Retrieve Emails Sent
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  reports/sent:
    get:
      summary: Retrieve Emails Sent
      description: Retrieve Emails Sent
      operationId: getReportsSent
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
        name: startindex
        description: Number indicating where to begin reporting results
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