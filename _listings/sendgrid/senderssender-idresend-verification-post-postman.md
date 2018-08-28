{
  "info": {
    "name": "SendGrid Add Senders Sender  Resend Verification",
    "_postman_id": "0dba9619-0c89-446f-b3c1-e6f045e1b161",
    "description": "**This enpdoint allows you to resend a sender identity verification email.**\n\nSender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "948cc0e3-7e61-4656-82c3-42701b2176cf",
          "name": "senders.sender_id.resend_verification.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "senders/:sender_id/resend_verification"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sender_id",
                  "value": "sender_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "**This enpdoint allows you to resend a sender identity verification email"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54e8caf4-31b7-4821-b045-5d04ca212453"
            }
          ]
        }
      ]
    }
  ]
}