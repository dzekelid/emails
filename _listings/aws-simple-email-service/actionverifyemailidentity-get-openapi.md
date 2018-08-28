---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 0
info:
  title: AWS Simple Email Service API Verify Email Identity
  version: 1.0.0
  description: Verifies an email address.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SendEmail:
    get:
      summary: Send Email
      description: Composes an email message based on input data, and then immediately
        queues the message for sending.
      operationId: sendEmail
      x-api-path-slug: actionsendemail-get
      parameters:
      - in: query
        name: ConfigurationSetName
        description: The name of the configuration set to use when you send an email
          using SendEmail
        type: string
      - in: query
        name: Destination
        description: 'The destination for this email, composed of To:, CC:, and BCC:
          fields'
        type: string
      - in: query
        name: Message
        description: The message to be sent
        type: string
      - in: query
        name: ReplyToAddresses.member.N
        description: The reply-to email address(es) for the message
        type: string
      - in: query
        name: ReturnPath
        description: The email address to which bounces and complaints are to be forwarded
          when feedback forwarding is enabled
        type: string
      - in: query
        name: ReturnPathArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: Source
        description: The email address that is sending the email
        type: string
      - in: query
        name: SourceArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: Tags.member.N
        description: A list of tags, in the form of name/value pairs, to apply to
          an email that you send using SendEmail
        type: string
      responses:
        200:
          description: OK
      tags:
      - Email
  /?Action=SendRawEmail:
    get:
      summary: Send Raw Email
      description: Sends an email message, with header and content specified by the
        client.
      operationId: sendRawEmail
      x-api-path-slug: actionsendrawemail-get
      parameters:
      - in: query
        name: ConfigurationSetName
        description: The name of the configuration set to use when you send an email
          using SendRawEmail
        type: string
      - in: query
        name: Destinations.member.N
        description: 'A list of destinations for the message, consisting of To:, CC:,
          and BCC: addresses'
        type: string
      - in: query
        name: FromArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: RawMessage
        description: The raw text of the message
        type: string
      - in: query
        name: ReturnPathArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: Source
        description: The identitys email address
        type: string
      - in: query
        name: SourceArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: Tags.member.N
        description: A list of tags, in the form of name/value pairs, to apply to
          an email that you send using SendRawEmail
        type: string
      responses:
        200:
          description: OK
      tags:
      - Email
  /?Action=DeleteVerifiedEmailAddress:
    get:
      summary: Delete Verified Email Address
      description: Deletes the specified email address from the list of verified addresses.
      operationId: deleteVerifiedEmailAddress
      x-api-path-slug: actiondeleteverifiedemailaddress-get
      parameters:
      - in: query
        name: EmailAddress
        description: An email address to be removed from the list of verified addresses
        type: string
      responses:
        200:
          description: OK
      tags:
      - Verified Email Addresses
  /?Action=ListVerifiedEmailAddresses:
    get:
      summary: List Verified Email Addresses
      description: Returns a list containing all of the email addresses that have
        been verified.
      operationId: listVerifiedEmailAddresses
      x-api-path-slug: actionlistverifiedemailaddresses-get
      parameters:
      - in: query
        name: VerifiedEmailAddresses.member.N
        description: A list of email addresses that have been verified
        type: string
      responses:
        200:
          description: OK
      tags:
      - Verified Email Addresses
  /?Action=VerifyEmailAddress:
    get:
      summary: Verify Email Address
      description: Verifies an email address.
      operationId: verifyEmailAddress
      x-api-path-slug: actionverifyemailaddress-get
      parameters:
      - in: query
        name: EmailAddress
        description: The email address to be verified
        type: string
      responses:
        200:
          description: OK
      tags:
      - Email Addresses
  /?Action=VerifyEmailIdentity:
    get:
      summary: Verify Email Identity
      description: Verifies an email address.
      operationId: verifyEmailIdentity
      x-api-path-slug: actionverifyemailidentity-get
      parameters:
      - in: query
        name: EmailAddress
        description: The email address to be verified
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
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