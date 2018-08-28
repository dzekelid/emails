{
  "info": {
    "name": "SendGrid Get User Webhooks Parse Settings",
    "_postman_id": "7272de22-d450-4020-a522-532db8789c45",
    "description": "**This endpoint allows you to retrieve all of your current inbound parse settings.**\n\nThe inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "d08522bf-82f4-4621-a97a-d115289e28e2",
          "name": "user.webhooks.parse.settings.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/user/webhooks/parse/settings?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all of your current inbound parse settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8349327-346c-4370-a5be-ed70ac2a3876"
            }
          ]
        }
      ]
    }
  ]
}