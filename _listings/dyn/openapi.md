---
swagger: "2.0"
x-collection-name: Dyn
x-complete: 1
info:
  title: Dyn
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  reports/delivered:
    get:
      summary: Retrieve Emails Delivered
      description: Retrieve Emails Delivered
      operationId: getReportsDelivered
      x-api-path-slug: reportsdelivered-get
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
      - Retrieve
      - Emails
      - Delivered
  reports/delivered/count:
    get:
      summary: Retrieve Count of Emails Delivered
      description: Retrieve Count of Emails Delivered
      operationId: getReportsDeliveredCount
      x-api-path-slug: reportsdeliveredcount-get
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
      - Retrieve
      - Count
      - of
      - Emails
      - Delivered
  reports/sent:
    get:
      summary: Retrieve Emails Sent
      description: Retrieve Emails Sent
      operationId: getReportsSent
      x-api-path-slug: reportssent-get
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
      - Retrieve
      - Emails
      - Sent
  reports/sent/count:
    get:
      summary: Retrieve Count of Emails Sent
      description: Retrieve Count of Emails Sent
      operationId: getReportsSentCount
      x-api-path-slug: reportssentcount-get
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
      - Retrieve
      - Count
      - of
      - Emails
      - Sent
---