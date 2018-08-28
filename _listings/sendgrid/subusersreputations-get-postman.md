{
  "info": {
    "name": "SendGrid Get Subusers Reputations",
    "_postman_id": "6e9ebc5d-af1c-414a-ab8a-0b4e4e456c7e",
    "description": "Subuser sender reputations give a good idea how well a sender is doing with regards to how recipients and recipient servers react to the mail that is being received. When a bounce, spam report, or other negative action happens on a sent email, it will effect your sender rating.\n\nThis endpoint allows you to request the reputations for your subusers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "f6bccecf-2343-4128-881d-de3b72863c09",
          "name": "subusers.reputations.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/subusers/reputations?usernames=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Subuser sender reputations give a good idea how well a sender is doing with regards to how recipients and recipient servers react to the mail that is being received"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b04c023-8ae5-45af-a8d5-feb6310a9176"
            }
          ]
        }
      ]
    }
  ]
}