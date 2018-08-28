{
  "info": {
    "name": "SendGrid",
    "_postman_id": "8c58bc94-3dd6-4453-9400-5480dac4f46f",
    "description": "The SendGrid Web API V3 Documentation. This is the entirety of the documented v3 endpoints. We have updated all the descriptions, parameters, requests, and responses. Authentication Every endpoint requires Authentication in the form of an Authorization Header: Authorization: Bearer API_KEY",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "a882c9fa-78a9-4190-a863-35bf16c7da67",
          "name": "alerts.alert_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "alerts/:alert_id"
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
                  "id": "alert_id",
                  "value": "alert_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a specific alert"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29a1549c-48a2-44ed-8d13-34c5c0c42d7a"
            }
          ]
        }
      ]
    }
  ]
}