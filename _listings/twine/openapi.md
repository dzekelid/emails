swagger: "2.0"
x-collection-name: Twine
x-complete: 1
info:
  title: Twine
  description: -overviewthe-twine-health-api-is-restful-api--the-requests-and-responses-are-formated-according-to-the-json-apihttpjsonapi-orgformat1-0-specification-in-addition-to-this-documentation-we-also-provide-an-openapihttpsgithub-comoaiopenapispecificationblobmasterversions2-0-md-yaml-file-describing-the-api-twine-api-specificationswagger-yaml--authenticationauthentication-for-the-twine-api-is-based-on-the-oauth-2-0-authorization-frameworkhttpstools-ietf-orghtmlrfc6749--twine-currently-supports-grant-types-of-client-credentials-and-refresh-token-see-post-oauthtokenoperationcreatetoken-for-details-on-the-request-and-response-formats--redocinject-securitydefinitions-
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /email_history:
    get:
      summary: List email histories
      description: Get a list of email histories
      operationId: fetchEmailHistories
      x-api-path-slug: email-history-get
      parameters:
      - in: query
        name: filter[emailType]
        description: Type of email
      - in: query
        name: filter[receiver]
        description: Twine user id of email recipient
      - in: query
        name: filter[sender]
        description: Twine user id of email sender
      - in: query
        name: sort
        description: 'valid sorts:  * send_time - ascending by send_time  * -send_time
          - descending by send_time'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Email
      - Histories
  /email_history/{id}:
    get:
      summary: Get an email history
      description: Get an email history by id
      operationId: fetchEmailHistory
      x-api-path-slug: email-historyid-get
      parameters:
      - in: path
        name: id
        description: Email history identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Email
      - History