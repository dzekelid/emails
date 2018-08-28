---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft List email templates
  description: |-
    Fetches multiple email template records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/activities/emails.json:
    get:
      summary: List emails
      description: |-
        Fetches multiple email records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.activities.emails.json.get
      x-api-path-slug: v2activitiesemails-json-get
      parameters:
      - in: query
        name: bounced
        description: Filters emails by whether they have bounced or not
      - in: query
        name: ids
        description: IDs of emails to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Emails
  /v2/activities/emails/{id}.json:
    get:
      summary: Fetch an email
      description: Fetches an email, by ID only.
      operationId: v2.activities.emails.id.json.get
      x-api-path-slug: v2activitiesemailsid-json-get
      parameters:
      - in: path
        name: id
        description: Email ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Email
  /v2/email_templates.json:
    get:
      summary: List email templates
      description: |-
        Fetches multiple email template records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.email_templates.json.get
      x-api-path-slug: v2email-templates-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of email templates to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: linked_to_team_template
        description: Filters email templates by whether they are linked to a team
          template or not
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_used_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Email
      - Templates
  /v2/email_templates/{id}.json:
    get:
      summary: Fetch an email template
      description: Fetches an email template, by ID only.
      operationId: v2.email_templates.id.json.get
      x-api-path-slug: v2email-templatesid-json-get
      parameters:
      - in: path
        name: id
        description: EmailTemplate ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Email
      - Template
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