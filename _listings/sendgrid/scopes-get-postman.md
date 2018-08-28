{
  "info": {
    "name": "SendGrid Get Scopes",
    "_postman_id": "fb123441-9f0b-4e63-9ad8-ce2ecdc1cc09",
    "description": "**This endpoint returns a list of all scopes that this user has access to.**\n\nAPI Keys can be used to authenticate the use of [SendGrid???s v3 Web API](https://sendgrid.com/docs/API_Reference/Web_API_v3/index.html), or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html). API Keys may be assigned certain permissions, or scopes, that limit which API endpoints they are able to access. For a more detailed explanation of how you can use API Key permissios, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/api_keys.html#-API-Key-Permissions) or [Classroom](https://sendgrid.com/docs/Classroom/Basics/API/api_key_permissions.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "39a6e79b-eb86-4da0-9e9d-910d3c9bf02e",
          "name": "GET_scopes",
          "request": {
            "url": "http://api.sendgrid.com/v3/scopes?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint returns a list of all scopes that this user has access to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c11a3a02-e38e-4532-b0dd-36cc7a8cee50"
            }
          ]
        }
      ]
    }
  ]
}