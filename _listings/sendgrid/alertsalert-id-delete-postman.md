{
  "info": {
    "name": "SendGrid",
    "_postman_id": "3c028a9a-5fc7-47ef-b249-0e54c93ac509",
    "description": "The SendGrid Web API V3 Documentation. This is the entirety of the documented v3 endpoints. We have updated all the descriptions, parameters, requests, and responses. Authentication Every endpoint requires Authentication in the form of an Authorization Header: Authorization: Bearer API_KEY",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "2aaf960b-c9c0-44db-a438-62180ddfb4fe",
          "name": "alerts.alert_id.delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to delete an alert"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3af4c2ce-643f-47cc-90de-d2dc2261d776"
            }
          ]
        }
      ]
    }
  ]
}