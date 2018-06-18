---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  description: github-is-the-best-place-to-share-code-with-friends-coworkers-classmates-and-complete-strangers--over-24-million-people-use-github-to-build-amazing-things-together-across-67-million-repositories--with-the-collaborative-features-of-github-com-and-github-business-it-has-never-been-easier-for-individuals-and-teams-to-write-faster-better-code-
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/emails:
    delete:
      summary: Delete User Emails
      description: |-
        Delete email address(es).
        You can include a single email address or an array of addresses.
      operationId: delete-email-addressesyou-can-include-a-single-email-address-or-an-array-of-addresses
      x-api-path-slug: useremails-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
    get:
      summary: Get User Emails
      description: |-
        List email addresses for a user.
        In the final version of the API, this method will return an array of hashes
        with extended information for each email address indicating if the address
        has been verified and if it's primary email address for GitHub.
        Until API v3 is finalized, use the application/vnd.github.v3 media type to
        get other response format.
      operationId: list-email-addresses-for-a-userin-the-final-version-of-the-api-this-method-will-return-an-array-of-h
      x-api-path-slug: useremails-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
    post:
      summary: Add User Emails
      description: |-
        Add email address(es).
        You can post a single email address or an array of addresses.
      operationId: add-email-addressesyou-can-post-a-single-email-address-or-an-array-of-addresses
      x-api-path-slug: useremails-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
---