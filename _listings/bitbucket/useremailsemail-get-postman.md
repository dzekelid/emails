{
  "info": {
    "name": "Bitbucket Get User Emails Email",
    "_postman_id": "b1e116d1-e0c7-4f7f-81ae-c632724eb599",
    "description": "Returns details about a specific one of the authenticated user's\nemail addresses.\n\nDetails describe whether the address has been confirmed by the user and\nwhether it is the user's primary address or not.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "dea77caa-7571-4a72-8554-95b385b11d7c",
          "name": "getUserEmailsEmail",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "user/emails/:email"
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "email",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details about a specific one of the authenticated user's\nemail addresses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2dcdf5c2-896e-4ec2-a60e-83a38a56d160"
            }
          ]
        }
      ]
    }
  ]
}