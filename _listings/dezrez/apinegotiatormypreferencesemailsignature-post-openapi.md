---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Allows you to upload a document for use as email signature
  version: 1.0.0
  description: Allows you to upload a document for use as email signature.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/inboundlead/checkformatchinggroups:
    get:
      summary: Check for Matching groups for the given leads based on contact item
        values i.e. Emails and Phones.
      description: Check for matching groups for the given leads based on contact
        item values i.e. emails and phones..
      operationId: InboundLead_CheckForMatchingGroupsByleadIdBypageSizeBypageNumber
      x-api-path-slug: apiinboundleadcheckformatchinggroups-get
      parameters:
      - in: query
        name: leadId
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - CheckMatching
      - Groupsthe
      - Given
      - Leads
      - Based
      - "On"
      - Contact
      - Item
      - Values
      - I
      - E
      - ""
      - Emails
      - Phones
  /api/branding/uploademailtemplate:
    post:
      summary: Upload the data to create a Email Document Template for a Brand.
      description: Upload the data to create a email document template for a brand..
      operationId: Branding_UploadEmailTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploademailtemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - Email
      - Document
      - Templatea
      - Brand
  /api/credentials/emailsync/usernamepassword:
    get:
      summary: Gets Email Sync Security Credentials
      description: Gets email sync security credentials.
      operationId: Credentials_EmailSyncUsernamePasswordBycredentialDataContract.usernameBycredentialDataContract.passw
      x-api-path-slug: apicredentialsemailsyncusernamepassword-get
      parameters:
      - in: query
        name: credentialDataContract.password
      - in: query
        name: credentialDataContract.username
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Email
      - Sync
      - Security
      - Credentials
    post:
      summary: "Creates or Updates Email Sync Security Credentials\r\nThis also uses
        the credentials to do a quick check and see if they are working\r\nit will
        throw an internal server error if there is an issue with the connection\r\nbut
        this may be the server address (s"
      description: "Creates or updates email sync security credentials\r\nthis also
        uses the credentials to do a quick check and see if they are working\r\nit
        will throw an internal server error if there is an issue with the connection\r\nbut
        this may be the server address (s."
      operationId: Credentials_UpsertEmailSyncUsernamePasswordBycredentialDataContract
      x-api-path-slug: apicredentialsemailsyncusernamepassword-post
      parameters:
      - in: body
        name: credentialDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - S
      - Email
      - Sync
      - Security
      - "Credentials\r\nThis"
      - Also
      - Uses
      - Credentials
      - To
      - Do
      - Quick
      - Check
      - See
      - If
      - They
      - Are
      - "Working\r\nIt"
      - Will
      - Throw
      - Internal
      - Server
      - Error
      - If
      - There
      - Is
      - Issue
      - "Connection\r\nBut"
      - This
      - May
      - Be
      - Server
      - Address
      - (s
    delete:
      summary: Delete Email Sync For a User
      description: Delete email sync for a user.
      operationId: Credentials_DeleteEmailSyncUsernamePassword
      x-api-path-slug: apicredentialsemailsyncusernamepassword-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Email
      - Sync
      - User
  /api/documentgeneration/emailtemplates:
    get:
      summary: Returns a list of email templates associated to this agency
      description: Returns a list of email templates associated to this agency.
      operationId: DocumentGeneration_GetEmailTemplates
      x-api-path-slug: apidocumentgenerationemailtemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Email
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/group/{id}/sendemail:
    post:
      summary: To send an adhoc email to a group
      description: To send an adhoc email to a group.
      operationId: Group_SendEmailByidByemailDataContract
      x-api-path-slug: apigroupidsendemail-post
      parameters:
      - in: body
        name: emailDataContract
        description: Details of the email to send
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The group id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Adhoc
      - Email
      - To
      - Group
  /api/job/SendSystemEmail:
    post:
      summary: Sends a basic email to any specified party.
      description: Sends a basic email to any specified party..
      operationId: Job_SendSystemEmailBysendSystemEmail
      x-api-path-slug: apijobsendsystememail-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: sendSystemEmail
        description: The send system email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Basic
      - Email
      - To
      - Any
      - Specified
      - Party
  /api/negotiator/my/preferences/emailsignature:
    post:
      summary: Allows you to upload a document for use as email signature
      description: Allows you to upload a document for use as email signature.
      operationId: Negotiator_UploadEmailSignatureBydocumentDetailsContract
      x-api-path-slug: apinegotiatormypreferencesemailsignature-post
      parameters:
      - in: body
        name: documentDetailsContract
        description: Document details
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Documentuse
      - As
      - Email
      - Signature
  /api/people/findbyemail:
    get:
      summary: Returns a list of people that have the supplied email address.
      description: Returns a list of people that have the supplied email address..
      operationId: People_GetPeopleWithEmailAddressByemailAddress
      x-api-path-slug: apipeoplefindbyemail-get
      parameters:
      - in: query
        name: emailAddress
        description: The email address
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - People
      - That
      - Have
      - Supplied
      - Email
      - Address
  /api/role/{id}/boardrequest:
    post:
      summary: To send an board request email to a external provider
      description: To send an board request email to a external provider.
      operationId: Role_BoardRequestByidByupdateBoardRequestDataContract
      x-api-path-slug: apiroleidboardrequest-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: updateBoardRequestDataContract
        description: Details of the sms to send
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Board
      - Request
      - Email
      - To
      - External
      - Provider
  /api/sync/mailsync:
    post:
      summary: Syncronise Email with Rezi Events, attach documents etc
      description: Syncronise email with rezi events, attach documents etc.
      operationId: Sync_EmailBymailSyncDataContract
      x-api-path-slug: apisyncmailsync-post
      parameters:
      - in: body
        name: mailSyncDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Syncronise
      - Email
      - Rezi
      - Events
      - ""
      - Attach
      - Documents
      - Etc
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