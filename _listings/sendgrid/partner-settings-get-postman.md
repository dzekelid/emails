{
  "info": {
    "name": "SendGrid Get Partner Settings",
    "_postman_id": "ee1d2e0f-ba34-4551-a0e7-d643556cc4db",
    "description": "**This endpoint allows you to retrieve a list of all partner settings that you can enable.**\n\nOur partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "27000057-c45f-40f5-8df9-1e5609f94a38",
          "name": "GET_partner_settings",
          "request": {
            "url": "http://api.sendgrid.com/v3/partner_settings?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a list of all partner settings that you can enable"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1ed4d0c-f77f-443e-86d4-1b79488d75b7"
            }
          ]
        }
      ]
    }
  ]
}