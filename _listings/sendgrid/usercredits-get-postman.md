{
  "info": {
    "name": "SendGrid Get User Credits",
    "_postman_id": "44715823-ae21-412f-bf92-32f07b52613a",
    "description": "**This endpoint allows you to retrieve the current credit balance for your account.**\n\nYour monthly credit allotment limits the number of emails you may send before incurring overage charges. For more information about credits and billing, please visit our [Clssroom](https://sendgrid.com/docs/Classroom/Basics/Billing/billing_info_and_faqs.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "19bf4251-27de-4886-b1f6-ab013ae3a094",
          "name": "user.credits.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/user/credits?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve the current credit balance for your account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27d266d9-7605-4420-b61b-10510426f396"
            }
          ]
        }
      ]
    }
  ]
}