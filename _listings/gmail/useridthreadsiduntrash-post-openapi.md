---
swagger: "2.0"
x-collection-name: Gmail
x-complete: 0
info:
  title: Gmail UnTrash Threat
  description: Removes the specified thread from the trash.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /gmail/v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{userId}/drafts:
    get:
      summary: Get Drafts
      description: Lists the drafts in the user's mailbox.
      operationId: gmail.users.drafts.list
      x-api-path-slug: useriddrafts-get
      parameters:
      - in: query
        name: includeSpamTrash
        description: Include drafts from SPAM and TRASH in the results
      - in: query
        name: maxResults
        description: Maximum number of drafts to return
      - in: query
        name: pageToken
        description: Page token to retrieve a specific page of results in the list
      - in: query
        name: q
        description: Only return draft messages matching the specified query
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
    post:
      summary: Update Draft
      description: Creates a new draft with the DRAFT label.
      operationId: gmail.users.drafts.create
      x-api-path-slug: useriddrafts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/drafts/send:
    post:
      summary: Send Draft
      description: Sends the specified, existing draft to the recipients in the To,
        Cc, and Bcc headers.
      operationId: gmail.users.drafts.send
      x-api-path-slug: useriddraftssend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/drafts/{id}:
    delete:
      summary: Delete Draft
      description: Immediately and permanently deletes the specified draft. Does not
        simply trash it.
      operationId: gmail.users.drafts.delete
      x-api-path-slug: useriddraftsid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the draft to delete
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
    get:
      summary: Get Draft
      description: Gets the specified draft.
      operationId: gmail.users.drafts.get
      x-api-path-slug: useriddraftsid-get
      parameters:
      - in: query
        name: format
        description: The format to return the draft in
      - in: path
        name: id
        description: The ID of the draft to retrieve
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
    put:
      summary: Update Draft
      description: Replaces a draft's content.
      operationId: gmail.users.drafts.update
      x-api-path-slug: useriddraftsid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The ID of the draft to update
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages:
    get:
      summary: Get Message
      description: Lists the messages in the user's mailbox.
      operationId: gmail.users.messages.list
      x-api-path-slug: useridmessages-get
      parameters:
      - in: query
        name: includeSpamTrash
        description: Include messages from SPAM and TRASH in the results
      - in: query
        name: labelIds
        description: Only return messages with labels that match all of the specified
          label IDs
      - in: query
        name: maxResults
        description: Maximum number of messages to return
      - in: query
        name: pageToken
        description: Page token to retrieve a specific page of results in the list
      - in: query
        name: q
        description: Only return messages matching the specified query
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
    post:
      summary: Create Message
      description: Directly inserts a message into only this user's mailbox similar
        to IMAP APPEND, bypassing most scanning and classification. Does not send
        a message.
      operationId: gmail.users.messages.insert
      x-api-path-slug: useridmessages-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: deleted
        description: Mark the email as permanently deleted (not TRASH) and only visible
          in Google Vault to a Vault administrator
      - in: query
        name: internalDateSource
        description: Source for Gmails internal date of the message
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages/batchDelete:
    post:
      summary: Delete Messages
      description: Deletes many messages by message ID. Provides no guarantees that
        messages were not already deleted or even existed at all.
      operationId: gmail.users.messages.batchDelete
      x-api-path-slug: useridmessagesbatchdelete-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages/batchModify:
    post:
      summary: Update Label
      description: Modifies the labels on the specified messages.
      operationId: gmail.users.messages.batchModify
      x-api-path-slug: useridmessagesbatchmodify-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages/import:
    post:
      summary: Import Message
      description: Imports a message into only this user's mailbox, with standard
        email delivery scanning and classification similar to receiving via SMTP.
        Does not send a message.
      operationId: gmail.users.messages.import
      x-api-path-slug: useridmessagesimport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: deleted
        description: Mark the email as permanently deleted (not TRASH) and only visible
          in Google Vault to a Vault administrator
      - in: query
        name: internalDateSource
        description: Source for Gmails internal date of the message
      - in: query
        name: neverMarkSpam
        description: Ignore the Gmail spam classifier decision and never mark this
          email as SPAM in the mailbox
      - in: query
        name: processForCalendar
        description: Process calendar invites in the email and add any extracted meetings
          to the Google Calendar for this user
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages/send:
    post:
      summary: Send Message
      description: Sends the specified message to the recipients in the To, Cc, and
        Bcc headers.
      operationId: gmail.users.messages.send
      x-api-path-slug: useridmessagessend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages/{id}:
    delete:
      summary: Delete Message
      description: Immediately and permanently deletes the specified message. This
        operation cannot be undone. Prefer messages.trash instead.
      operationId: gmail.users.messages.delete
      x-api-path-slug: useridmessagesid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the message to delete
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
    get:
      summary: Get Message
      description: Gets the specified message.
      operationId: gmail.users.messages.get
      x-api-path-slug: useridmessagesid-get
      parameters:
      - in: query
        name: format
        description: The format to return the message in
      - in: path
        name: id
        description: The ID of the message to retrieve
      - in: query
        name: metadataHeaders
        description: When given and format is METADATA, only include headers specified
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages/{id}/modify:
    post:
      summary: Modify message
      description: Modifies the labels on the specified message.
      operationId: gmail.users.messages.modify
      x-api-path-slug: useridmessagesidmodify-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The ID of the message to modify
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages/{id}/trash:
    post:
      summary: Trash Message
      description: Moves the specified message to the trash.
      operationId: gmail.users.messages.trash
      x-api-path-slug: useridmessagesidtrash-post
      parameters:
      - in: path
        name: id
        description: The ID of the message to Trash
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages/{id}/untrash:
    post:
      summary: UnTrash Message
      description: Removes the specified message from the trash.
      operationId: gmail.users.messages.untrash
      x-api-path-slug: useridmessagesiduntrash-post
      parameters:
      - in: path
        name: id
        description: The ID of the message to remove from Trash
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/messages/{messageId}/attachments/{id}:
    get:
      summary: Get Attachments
      description: Gets the specified message attachment.
      operationId: gmail.users.messages.attachments.get
      x-api-path-slug: useridmessagesmessageidattachmentsid-get
      parameters:
      - in: path
        name: id
        description: The ID of the attachment
      - in: path
        name: messageId
        description: The ID of the message containing the attachment
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email
  /{userId}/threads:
    get:
      summary: Get Threads
      description: Lists the threads in the user's mailbox.
      operationId: gmail.users.threads.list
      x-api-path-slug: useridthreads-get
      parameters:
      - in: query
        name: includeSpamTrash
        description: Include threads from SPAM and TRASH in the results
      - in: query
        name: labelIds
        description: Only return threads with labels that match all of the specified
          label IDs
      - in: query
        name: maxResults
        description: Maximum number of threads to return
      - in: query
        name: pageToken
        description: Page token to retrieve a specific page of results in the list
      - in: query
        name: q
        description: Only return threads matching the specified query
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email Thread
  /{userId}/threads/{id}:
    delete:
      summary: Delete Threads
      description: Immediately and permanently deletes the specified thread. This
        operation cannot be undone. Prefer threads.trash instead.
      operationId: gmail.users.threads.delete
      x-api-path-slug: useridthreadsid-delete
      parameters:
      - in: path
        name: id
        description: ID of the Thread to delete
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email Thread
    get:
      summary: Get Threads
      description: Gets the specified thread.
      operationId: gmail.users.threads.get
      x-api-path-slug: useridthreadsid-get
      parameters:
      - in: query
        name: format
        description: The format to return the messages in
      - in: path
        name: id
        description: The ID of the thread to retrieve
      - in: query
        name: metadataHeaders
        description: When given and format is METADATA, only include headers specified
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email Thread
  /{userId}/threads/{id}/modify:
    post:
      summary: Modify Thread labels
      description: Modifies the labels applied to the thread. This applies to all
        messages in the thread.
      operationId: gmail.users.threads.modify
      x-api-path-slug: useridthreadsidmodify-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The ID of the thread to modify
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email Thread
  /{userId}/threads/{id}/trash:
    post:
      summary: Trash Thread
      description: Moves the specified thread to the trash.
      operationId: gmail.users.threads.trash
      x-api-path-slug: useridthreadsidtrash-post
      parameters:
      - in: path
        name: id
        description: The ID of the thread to Trash
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email Thread
  /{userId}/threads/{id}/untrash:
    post:
      summary: UnTrash Threat
      description: Removes the specified thread from the trash.
      operationId: gmail.users.threads.untrash
      x-api-path-slug: useridthreadsiduntrash-post
      parameters:
      - in: path
        name: id
        description: The ID of the thread to remove from Trash
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Email Thread
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