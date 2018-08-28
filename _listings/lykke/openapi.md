swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Email/PrivateWalletAddress:
    post:
      summary: Add API Email Privatewalletaddress
      description: Add api email privatewalletaddress.
      operationId: ApiEmailPrivateWalletAddressPost
      x-api-path-slug: apiemailprivatewalletaddress-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Privatewalletaddress
  /api/EmailMeWalletAddress:
    post:
      summary: Add API Emailmewalletaddress
      description: Add api emailmewalletaddress.
      operationId: ApiEmailMeWalletAddressPost
      x-api-path-slug: apiemailmewalletaddress-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: reqModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Emailmewalletaddress
  /api/EmailVerification:
    get:
      summary: Get API Emailverification
      description: Get api emailverification.
      operationId: ApiEmailVerificationGet
      x-api-path-slug: apiemailverification-get
      parameters:
      - in: query
        name: code
      - in: query
        name: email
      - in: query
        name: partnerId
      responses:
        200:
          description: OK
      tags:
      - Emailverification
    post:
      summary: Add API Emailverification
      description: Add api emailverification.
      operationId: ApiEmailVerificationPost
      x-api-path-slug: apiemailverification-post
      parameters:
      - in: body
        name: email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Emailverification
  /api/MyLykkeCashInEmail:
    post:
      summary: Add API Mylykkecashinemail
      description: Add api mylykkecashinemail.
      operationId: ApiMyLykkeCashInEmailPost
      x-api-path-slug: apimylykkecashinemail-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: reqModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Mylykkecashinemail
  /api/RemindPasswordEmail:
    post:
      summary: Add API Remindpasswordemail
      description: Add api remindpasswordemail.
      operationId: ApiRemindPasswordEmailPost
      x-api-path-slug: apiremindpasswordemail-post
      parameters:
      - in: body
        name: reqModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Remindpasswordemail
  /api/SendBlockchainEmail:
    post:
      summary: Add API Sendblockchainemail
      description: Add api sendblockchainemail.
      operationId: ApiSendBlockchainEmailPost
      x-api-path-slug: apisendblockchainemail-post
      parameters:
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Sendblockchainemail