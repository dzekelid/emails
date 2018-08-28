{
  "info": {
    "name": "SendGrid Get User Webhooks Parse Stats",
    "_postman_id": "ac68c395-b785-4f14-beac-73d9cc431f4d",
    "description": "**This endpoint allows you to retrieve the statistics for your Parse Webhook useage.**\n\nSendGrid's Inbound Parse Webhook allows you to parse the contents and attachments of incomming emails. The Parse API can then POST the parsed emails to a URL that you specify. The Inbound Parse Webhook cannot parse messages greater than 20MB in size, including all attachments.\n\nThere are a number of pre-made integrations for the SendGrid Parse Webhook which make processing events easy. You can find these integrations in the [Library Index](https://sendgrid.com/docs/Integrate/libraries.html#-Webhook-Libraries).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "95a0d7ba-0f0b-4cf3-8f08-5470d3218d6a",
          "name": "user.webhooks.parse.stats.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/user/webhooks/parse/stats?aggregated_by=%7B%7D&end_date=%7B%7D&limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D&start_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve the statistics for your Parse Webhook useage"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4e1c597-0bfd-4f98-9cf9-3a553a834869"
            }
          ]
        }
      ]
    }
  ]
}