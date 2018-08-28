{
  "info": {
    "name": "SendGrid Get Templates",
    "_postman_id": "06f3dc7d-0479-469b-b174-d93c48b88bcc",
    "description": "**This endpoint allows you to retrieve all transactional templates.**\n\nEach user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.\n\nTransactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "f76f7641-f2c4-41c0-b57f-7d9fc1f4bfbd",
          "name": "GET_templates",
          "request": {
            "url": "http://api.sendgrid.com/v3/templates?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all transactional templates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "765c6221-c02d-45a4-945f-a1b80f738b00"
            }
          ]
        }
      ]
    }
  ]
}