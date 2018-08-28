---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Post Users Emails
  version: 1.0.0
  description: Add an email address to a specified user. Available only for admins.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/services/emails-on-push:
    put:
      summary: Put Projects Services Emails On Push
      description: Set emails-on-push service for project
      operationId: putV3ProjectsIdServicesEmailsOnPush
      x-api-path-slug: v3projectsidservicesemailsonpush-put
      parameters:
      - in: formData
        name: disable_diffs
        description: Disable code diffs
      - in: path
        name: id
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: recipients
        description: Comma-separated list of recipient email addresses
      - in: formData
        name: send_from_committer_email
        description: Send from committer
      - in: formData
        name: tag_push_events
        description: Event will be triggered when a new tag is pushed to the repository
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Emails
      - "On"
      - Push
  /v3/users/{id}/emails:
    post:
      summary: Post Users Emails
      description: Add an email address to a specified user. Available only for admins.
      operationId: postV3UsersIdEmails
      x-api-path-slug: v3usersidemails-post
      parameters:
      - in: formData
        name: email
        description: The email of the user
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Emails
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