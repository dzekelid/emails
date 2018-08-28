---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Put Projects Services Pipelines Email
  version: 1.0.0
  description: Set pipelines-email service for project
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
    get:
      summary: Get Users Emails
      description: Get the emails addresses of a specified user. Available only for
        admins.
      operationId: getV3UsersIdEmails
      x-api-path-slug: v3usersidemails-get
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Emails
  /v3/users/{id}/emails/{email_id}:
    delete:
      summary: Delete Users Emails Email
      description: Delete an email address of a specified user. Available only for
        admins.
      operationId: deleteV3UsersIdEmailsEmailId
      x-api-path-slug: v3usersidemailsemail-id-delete
      parameters:
      - in: path
        name: email_id
        description: The ID of the email
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Emails
      - Email
  /v3/user/emails:
    get:
      summary: Get User Emails
      description: Get the currently authenticated user's email addresses
      operationId: getV3UserEmails
      x-api-path-slug: v3useremails-get
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
    post:
      summary: Post User Emails
      description: Add new email address to the currently authenticated user
      operationId: postV3UserEmails
      x-api-path-slug: v3useremails-post
      parameters:
      - in: formData
        name: email
        description: The new email
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
  /v3/user/emails/{email_id}:
    get:
      summary: Get User Emails Email
      description: Get a single email address owned by the currently authenticated
        user
      operationId: getV3UserEmailsEmailId
      x-api-path-slug: v3useremailsemail-id-get
      parameters:
      - in: path
        name: email_id
        description: The ID of the email
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
      - Email
    delete:
      summary: Delete User Emails Email
      description: Delete an email address from the currently authenticated user
      operationId: deleteV3UserEmailsEmailId
      x-api-path-slug: v3useremailsemail-id-delete
      parameters:
      - in: path
        name: email_id
        description: The ID of the email
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
      - Email
  /v3/projects/{id}/services/builds-email:
    put:
      summary: Put Projects Services Builds Email
      description: Set builds-email service for project
      operationId: putV3ProjectsIdServicesBuildsEmail
      x-api-path-slug: v3projectsidservicesbuildsemail-put
      parameters:
      - in: formData
        name: add_pusher
        description: Add pusher to recipients list
      - in: formData
        name: build_events
        description: Event will be triggered when a build status changes
      - in: path
        name: id
      - in: formData
        name: notify_only_broken_builds
        description: Notify only broken builds
      - in: formData
        name: recipients
        description: Comma-separated list of recipient email addresses
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Builds
      - Email
  /v3/projects/{id}/services/pipelines-email:
    put:
      summary: Put Projects Services Pipelines Email
      description: Set pipelines-email service for project
      operationId: putV3ProjectsIdServicesPipelinesEmail
      x-api-path-slug: v3projectsidservicespipelinesemail-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: notify_only_broken_builds
        description: Notify only broken builds
      - in: formData
        name: pipeline_events
      - in: formData
        name: recipients
        description: Comma-separated list of recipient email addresses
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Pipelines
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