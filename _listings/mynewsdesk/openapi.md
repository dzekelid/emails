swagger: "2.0"
x-collection-name: Mynewsdesk
x-complete: 1
info:
  title: My News Desk Pressroom List
  description: mynewsdesk-webservice-for-newsroom-is-a-way-for-you-as-a-registered-customer-to-fetch-information-from-your-newsroom-at-mynewsdesk-to-any-system--you-can-get-all-your-information-as-xml-and-create-email-subscriptions-to-your-material-
  termsOfService: http://www.mynewsdesk.com/about/terms-and-conditions?locale=en
  version: v1
host: www.mynewsdesk.com
basePath: /services/pressroom/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  send_email/:
    get:
      summary: Send Email
      description: Send Email
      operationId: getSendEmail
      x-api-path-slug: send-email-get
      parameters:
      - in: query
        name: from
        description: Name of sender
      - in: query
        name: item_id
        description: ID of the material to be fetched
      - in: query
        name: message
        description: Personal message from the sender to the recipient
      - in: query
        name: to_email
        description: Recipient email address
      - in: query
        name: type_of_media
        description: The type of material to be fetched
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - Send
      - Email