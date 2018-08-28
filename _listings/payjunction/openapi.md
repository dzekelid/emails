swagger: "2.0"
x-collection-name: PayJunction
x-complete: 1
info:
  title: PayJunction API Basic
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transactions/{transactionId}/receipts/latest/email:
    post:
      summary: Post Transactions Receipts Latest Email
      description: /transactions/{transactionid}/receipts/latest/email.
      operationId: TransactionsReceiptsLatestEmailByTransactionIdPost
      x-api-path-slug: transactionstransactionidreceiptslatestemail-post
      parameters:
      - in: formData
        name: replyTo
      - in: formData
        name: requestSignature
      - in: formData
        name: to
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Latest
      - Email