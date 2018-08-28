swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 1
info:
  title: Kentico Cloud
  description: this-is-a-collection-of-resources-you-can-find-within-the-kentico-cloud-developer-hubhttpsdeveloper-kenticocloud-com--kentico-cloudhttpskenticocloud-com-is-a-cloudfirst-headless-cms-that-allows-you-to-distribute-content-to-any-channel-and-device-websites-mobile-devices-mixed-reality-devices-presentation-kiosks-etc--through-an-api-certain-apis-require-that-you-include-the-authorization-header--find-more-in-httpsdeveloper-kenticocloud-comreferenceauthentication-
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /email/lola.mira@blabla.com:
    get:
      summary: View data of visitor by email
      description: ""
      operationId: EmailLolaMiraBlablaComGet
      x-api-path-slug: emaillola-mirablabla-com-get
      responses:
        200:
          description: OK
      tags:
      - View
      - Data
      - Of
      - Visitor
      - By
      - Email
    delete:
      summary: Delete data of visitor by email
      description: ""
      operationId: EmailLolaMiraBlablaComDelete
      x-api-path-slug: emaillola-mirablabla-com-delete
      responses:
        200:
          description: OK
      tags:
      - Data
      - Of
      - Visitor
      - By
      - Email