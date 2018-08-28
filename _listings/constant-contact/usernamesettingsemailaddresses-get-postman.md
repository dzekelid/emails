{
  "info": {
    "name": "Constant Contact List Account Email Addresses",
    "_postman_id": "559373bf-2295-4359-bf5d-fcfe1017b781",
    "description": "List Account Email Addresses",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "1c606502-d5c7-4cf4-8554-66a4be6fd69d",
          "name": "list-account-email-addresses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/settings/emailaddresses"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List Account Email Addresses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa71d686-1dbf-4d5f-8b5a-8291a2797305"
            }
          ]
        }
      ]
    }
  ]
}