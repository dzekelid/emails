---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get User Inbox Unread
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method is effectively
    an alias for /inbox/unread. It is provided for consumers who make strong assumptions
    about operating within the context of a single site rather than the Stack Exchange
    network as a whole.\n \n{id} can contain a single id, to find it programatically
    look for user_id on user or shallow_user objects.\n \nThis method returns a list
    of inbox items."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /inbox:
    get:
      summary: Get Inbox
      description: "Returns a user's inbox.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method returns a list of
        inbox items."
      operationId: returns-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containing-read-inbox-this-m
      x-api-path-slug: inbox-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Email
      - Inbox
  /inbox/unread:
    get:
      summary: Unread Inbox
      description: "Returns the unread items in a user's inbox.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
        a list of inbox items."
      operationId: returns-the-unread-items-in-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containi
      x-api-path-slug: inboxunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: since
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Email
      - Inbox
  /me/inbox:
    get:
      summary: My Inbox
      description: "Returns the user identified by access_token's inbox.\n \nThis
        method requires an access_token, with a scope containing \"read_inbox\".\n
        \nThis method returns a list of inbox items."
      operationId: returns-the-user-identified-by-access-tokens-inbox-this-method-requires-an-access-token-with-a-scope
      x-api-path-slug: meinbox-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Email
      - Inbox
  /me/inbox/unread:
    get:
      summary: My Inbox Unread
      description: "Returns the unread items in the user identified by access_token's
        inbox.\n \nThis method requires an access_token, with a scope containing \"read_inbox\".\n
        \nThis method returns a list of inbox items."
      operationId: returns-the-unread-items-in-the-user-identified-by-access-tokens-inbox-this-method-requires-an-acces
      x-api-path-slug: meinboxunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: since
        description: Unix date
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Email
      - Inbox
  /users/{id}/inbox:
    get:
      summary: Get User Inbox
      description: "Returns a user's inbox.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method is effectively an
        alias for /inbox. It is provided for consumers who make strong assumptions
        about operating within the context of a single site rather than the Stack
        Exchange network as a whole.\n \n{id} can contain a single id, to find it
        programatically look for user_id on user or shallow_user objects.\n \nThis
        method returns a list of inbox items."
      operationId: returns-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containing-read-inbox-this-m
      x-api-path-slug: usersidinbox-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Email
      - Inbox
  /users/{id}/inbox/unread:
    get:
      summary: Get User Inbox Unread
      description: "Returns the unread items in a user's inbox.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method is
        effectively an alias for /inbox/unread. It is provided for consumers who make
        strong assumptions about operating within the context of a single site rather
        than the Stack Exchange network as a whole.\n \n{id} can contain a single
        id, to find it programatically look for user_id on user or shallow_user objects.\n
        \nThis method returns a list of inbox items."
      operationId: returns-the-unread-items-in-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containi
      x-api-path-slug: usersidinboxunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: since
        description: Unix date
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Email
      - Inbox
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