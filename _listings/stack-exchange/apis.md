---
name: Stack Exchange
x-slug: stack-exchange
description: After someone asks a question, members of the community propose answers.
  Others vote on those answers. Very quickly, the answers with the most votes rise
  to the top. You dont have to read through a lot of discussion to find the best answer.    Like
  to...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
x-kinRank: "8"
x-alexaRank: "126"
tags: Emails
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange - Get Inbox
  x-api-slug: inbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-openapi.md
- name: Stack Exchange - Unread Inbox
  x-api-slug: inboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
    a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-openapi.md
- name: Stack Exchange - My Inbox
  x-api-slug: meinbox-get
  description: "Returns the user identified by access_token's inbox.\n \nThis method
    requires an access_token, with a scope containing \"read_inbox\".\n \nThis method
    returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-openapi.md
- name: Stack Exchange - My Inbox Unread
  x-api-slug: meinboxunread-get
  description: "Returns the unread items in the user identified by access_token's
    inbox.\n \nThis method requires an access_token, with a scope containing \"read_inbox\".\n
    \nThis method returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-openapi.md
- name: Stack Exchange - Get User Inbox
  x-api-slug: usersidinbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method is effectively an alias
    for /inbox. It is provided for consumers who make strong assumptions about operating
    within the context of a single site rather than the Stack Exchange network as
    a whole.\n \n{id} can contain a single id, to find it programatically look for
    user_id on user or shallow_user objects.\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-openapi.md
- name: Stack Exchange - Get User Inbox Unread
  x-api-slug: usersidinboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method is effectively
    an alias for /inbox/unread. It is provided for consumers who make strong assumptions
    about operating within the context of a single site rather than the Stack Exchange
    network as a whole.\n \n{id} can contain a single id, to find it programatically
    look for user_id on user or shallow_user objects.\n \nThis method returns a list
    of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-openapi.md
- name: Stack Exchange - Get Inbox
  x-api-slug: inbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-openapi.md
- name: Stack Exchange - Get Inbox
  x-api-slug: inbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-openapi.md
- name: Stack Exchange - Unread Inbox
  x-api-slug: inboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
    a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-openapi.md
- name: Stack Exchange - Get Inbox
  x-api-slug: inbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-openapi.md
- name: Stack Exchange - Unread Inbox
  x-api-slug: inboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
    a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-openapi.md
- name: Stack Exchange - My Inbox
  x-api-slug: meinbox-get
  description: "Returns the user identified by access_token's inbox.\n \nThis method
    requires an access_token, with a scope containing \"read_inbox\".\n \nThis method
    returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-openapi.md
- name: Stack Exchange - Unread Inbox
  x-api-slug: inboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
    a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-openapi.md
- name: Stack Exchange - My Inbox
  x-api-slug: meinbox-get
  description: "Returns the user identified by access_token's inbox.\n \nThis method
    requires an access_token, with a scope containing \"read_inbox\".\n \nThis method
    returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-openapi.md
- name: Stack Exchange - My Inbox Unread
  x-api-slug: meinboxunread-get
  description: "Returns the unread items in the user identified by access_token's
    inbox.\n \nThis method requires an access_token, with a scope containing \"read_inbox\".\n
    \nThis method returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-openapi.md
- name: Stack Exchange - My Inbox
  x-api-slug: meinbox-get
  description: "Returns the user identified by access_token's inbox.\n \nThis method
    requires an access_token, with a scope containing \"read_inbox\".\n \nThis method
    returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-openapi.md
- name: Stack Exchange - My Inbox Unread
  x-api-slug: meinboxunread-get
  description: "Returns the unread items in the user identified by access_token's
    inbox.\n \nThis method requires an access_token, with a scope containing \"read_inbox\".\n
    \nThis method returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-openapi.md
- name: Stack Exchange - Get User Inbox
  x-api-slug: usersidinbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method is effectively an alias
    for /inbox. It is provided for consumers who make strong assumptions about operating
    within the context of a single site rather than the Stack Exchange network as
    a whole.\n \n{id} can contain a single id, to find it programatically look for
    user_id on user or shallow_user objects.\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-openapi.md
- name: Stack Exchange - My Inbox Unread
  x-api-slug: meinboxunread-get
  description: "Returns the unread items in the user identified by access_token's
    inbox.\n \nThis method requires an access_token, with a scope containing \"read_inbox\".\n
    \nThis method returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-openapi.md
- name: Stack Exchange - Get User Inbox
  x-api-slug: usersidinbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method is effectively an alias
    for /inbox. It is provided for consumers who make strong assumptions about operating
    within the context of a single site rather than the Stack Exchange network as
    a whole.\n \n{id} can contain a single id, to find it programatically look for
    user_id on user or shallow_user objects.\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-openapi.md
- name: Stack Exchange - Get User Inbox Unread
  x-api-slug: usersidinboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method is effectively
    an alias for /inbox/unread. It is provided for consumers who make strong assumptions
    about operating within the context of a single site rather than the Stack Exchange
    network as a whole.\n \n{id} can contain a single id, to find it programatically
    look for user_id on user or shallow_user objects.\n \nThis method returns a list
    of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-openapi.md
- name: Stack Exchange - Get User Inbox
  x-api-slug: usersidinbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method is effectively an alias
    for /inbox. It is provided for consumers who make strong assumptions about operating
    within the context of a single site rather than the Stack Exchange network as
    a whole.\n \n{id} can contain a single id, to find it programatically look for
    user_id on user or shallow_user objects.\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-openapi.md
- name: Stack Exchange - Get User Inbox Unread
  x-api-slug: usersidinboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method is effectively
    an alias for /inbox/unread. It is provided for consumers who make strong assumptions
    about operating within the context of a single site rather than the Stack Exchange
    network as a whole.\n \n{id} can contain a single id, to find it programatically
    look for user_id on user or shallow_user objects.\n \nThis method returns a list
    of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-openapi.md
- name: Stack Exchange - Get User Inbox Unread
  x-api-slug: usersidinboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method is effectively
    an alias for /inbox/unread. It is provided for consumers who make strong assumptions
    about operating within the context of a single site rather than the Stack Exchange
    network as a whole.\n \n{id} can contain a single id, to find it programatically
    look for user_id on user or shallow_user objects.\n \nThis method returns a list
    of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-openapi.md
- name: Stack Exchange - Get User Inbox Unread
  x-api-slug: usersidinboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method is effectively
    an alias for /inbox/unread. It is provided for consumers who make strong assumptions
    about operating within the context of a single site rather than the Stack Exchange
    network as a whole.\n \n{id} can contain a single id, to find it programatically
    look for user_id on user or shallow_user objects.\n \nThis method returns a list
    of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinboxunread-get-openapi.md
- name: Stack Exchange - Get User Inbox
  x-api-slug: usersidinbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method is effectively an alias
    for /inbox. It is provided for consumers who make strong assumptions about operating
    within the context of a single site rather than the Stack Exchange network as
    a whole.\n \n{id} can contain a single id, to find it programatically look for
    user_id on user or shallow_user objects.\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/usersidinbox-get-openapi.md
- name: Stack Exchange - My Inbox Unread
  x-api-slug: meinboxunread-get
  description: "Returns the unread items in the user identified by access_token's
    inbox.\n \nThis method requires an access_token, with a scope containing \"read_inbox\".\n
    \nThis method returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinboxunread-get-openapi.md
- name: Stack Exchange - My Inbox
  x-api-slug: meinbox-get
  description: "Returns the user identified by access_token's inbox.\n \nThis method
    requires an access_token, with a scope containing \"read_inbox\".\n \nThis method
    returns a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/meinbox-get-openapi.md
- name: Stack Exchange - Unread Inbox
  x-api-slug: inboxunread-get
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
    a list of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inboxunread-get-openapi.md
- name: Stack Exchange - Get Inbox
  x-api-slug: inbox-get
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/stack-exchange/inbox-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://square.api.gallery.streamdata.io
- type: x-api-stack
  url: http://stack.exchange.stack.network
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-crunchbase
  url: https://crunchbase.com/organization/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: legal@stackexchange.com
- type: x-email
  url: team@stackexchange.com
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-linkedin
  url: https://www.linkedin.com/company/stack-exchange
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: http://stackexchange.com
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---