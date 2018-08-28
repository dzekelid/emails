swagger: "2.0"
x-collection-name: NPR
x-complete: 1
info:
  title: NPR One API Reference
  description: npr-one-is-a-smart-application-that-brings-the-best-of-npr-and-member-station-programming-newscasts-podcasts-and-stories-together-to-create-a-new-experience-for-listening--it-provides-an-editorcurated-and-localized-mobile-listening-experience-based-on-the-content-the-listener-chooses-likes-shares-and-enjoys--the-api-provides-all-of-the-content-and-customization-in-a-simple-structured-way-that-is-easy-for-applicationdevelopers-to-implement-
  termsOfService: http://dev.npr.org/develop/terms-of-use
  contact:
    name: NPR One Enterprise Team
    url: http://dev.npr.org
    email: NPROneEnterprise@npr.org
  version: 1.0.0
host: api.npr.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /localactivation/v2/donate_email:
    get:
      summary: Send a donation email to the logged-in user (only on request)
      description: This will send a station-specific donation email to the logged-in
        user.
      operationId: sendDonationEmail
      x-api-path-slug: localactivationv2donate-email-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - News
      - Localactivation
      - Donate
      - Email