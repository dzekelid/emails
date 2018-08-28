{
  "info": {
    "name": "SendGrid",
    "_postman_id": "3eb844e9-d6cc-4113-b5a4-fa0dc67ac015",
    "description": "The SendGrid Web API V3 Documentation. This is the entirety of the documented v3 endpoints. We have updated all the descriptions, parameters, requests, and responses. Authentication Every endpoint requires Authentication in the form of an Authorization Header: Authorization: Bearer API_KEY",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "d7b367ea-c414-45e4-a142-6b54ed25db2e",
          "name": "tracking_settings.google_analytics.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/tracking_settings/google_analytics?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current setting for Google Analytics"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b74eca0d-dfa7-4dc6-88e8-8645dfaa5d83"
            }
          ]
        }
      ]
    }
  ]
}