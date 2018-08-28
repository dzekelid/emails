{
  "info": {
    "name": "SendGrid Get Senders",
    "_postman_id": "ff12726c-6cc0-4d2f-af1a-1c253eab0eaa",
    "description": "**This endpoint allows you to retrieve a list of all sender identities that have been created for your account.**\n\nSender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "de9b94c9-49c8-4522-bf45-67535078307f",
          "name": "senders.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/senders?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a list of all sender identities that have been created for your account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b86339a-8c65-4f1b-9b9a-4c37d4ae4eef"
            }
          ]
        }
      ]
    }
  ]
}