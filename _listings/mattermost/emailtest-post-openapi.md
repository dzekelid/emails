---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Send a test email
  description: |-
    Send a test email to make sure you have your email settings configured correctly. Optionally provide a configuration in the request body to test. If no valid configuration is present in the request body the current server configuration will be tested.
    ##### Permissions
    Must have `manage_system` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/password/reset/send:
    post:
      summary: Send password reset email
      description: |-
        Send an email containing a link for resetting the user's password. The link will contain a one-use, timed recovery code tied to the user's account. Only works for non-SSO users.
        ##### Permissions
        No permissions required.
      operationId: send-an-email-containing-a-link-for-resetting-the-users-password-the-link-will-contain-a-oneuse-time
      x-api-path-slug: userspasswordresetsend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Password
      - Reset
      - Email
  /users/email/{email}:
    get:
      summary: Get a user by email
      description: |-
        Get a user object by providing a user email. Sensitive information will be sanitized out.
        ##### Permissions
        Requires an active session but no other permissions.
      operationId: get-a-user-object-by-providing-a-user-email-sensitive-information-will-be-sanitized-out-permissionsr
      x-api-path-slug: usersemailemail-get
      parameters:
      - in: path
        name: email
        description: User Email
      responses:
        200:
          description: OK
      tags:
      - User
      - By
      - Email
  /users/email/verify:
    post:
      summary: Verify user email
      description: |-
        Verify the email used by a user to sign-up their account with.
        ##### Permissions
        No permissions required.
      operationId: verify-the-email-used-by-a-user-to-signup-their-account-with-permissionsno-permissions-required
      x-api-path-slug: usersemailverify-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Verify
      - User
      - Email
  /users/email/verify/send:
    post:
      summary: Send verification email
      description: |-
        Send an email with a verification link to a user that has an email matching the one in the request body. This endpoint will return success even if the email does not match any users on the system.
        ##### Permissions
        No permissions required.
      operationId: send-an-email-with-a-verification-link-to-a-user-that-has-an-email-matching-the-one-in-the-request-b
      x-api-path-slug: usersemailverifysend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Verification
      - Email
  /teams/{team_id}/invite/email:
    post:
      summary: Invite users to the team by email
      description: |-
        Invite users to the existing team usign the user's email.
        ##### Permissions
        Must have `invite_to_team` permission for the team.
      operationId: invite-users-to-the-existing-team-usign-the-users-email-permissionsmust-have-invite-to-team-permissi
      x-api-path-slug: teamsteam-idinviteemail-post
      parameters:
      - in: body
        name: body
        description: List of users email
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Invite
      - Users
      - To
      - Team
      - By
      - Email
  /email/test:
    post:
      summary: Send a test email
      description: |-
        Send a test email to make sure you have your email settings configured correctly. Optionally provide a configuration in the request body to test. If no valid configuration is present in the request body the current server configuration will be tested.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: send-a-test-email-to-make-sure-you-have-your-email-settings-configured-correctly-optionally-provide-
      x-api-path-slug: emailtest-post
      parameters:
      - in: body
        name: body
        description: Mattermost configuration
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Test
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