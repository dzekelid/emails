{
  "info": {
    "name": "SendGrid Get Contactdb Recipients Billable Count",
    "_postman_id": "f51da0d7-bf20-48a8-a266-84c3c1e2d6f6",
    "description": "**This endpoint allows you to retrieve the number of Marketing Campaigns recipients that you will be billed for.**\n\nYou are billed for marketing campaigns based on the highest number of recipients you have had in your account at one time. This endpoint will allow you to know the current billable count value.\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "dce9a347-0157-4ba4-9402-90ac345b9125",
          "name": "contactdb.recipients.billable_count.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/contactdb/recipients/billable_count?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve the number of Marketing Campaigns recipients that you will be billed for"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8932489b-975e-4aef-9784-b1025234cfc7"
            }
          ]
        }
      ]
    }
  ]
}