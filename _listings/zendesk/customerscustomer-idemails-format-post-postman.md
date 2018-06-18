{
  "info": {
    "name": "Sales Force Desk API Create Customer Email",
    "_postman_id": "8db7255e-33af-48ff-91c6-b8eb2ceadc5d",
    "description": "Create customer email.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Customers",
      "item": [
        {
          "id": "81cebe70-d73d-4029-b91c-b7908d6f9b84",
          "name": "get-customers",
          "request": {
            "url": "http://yoursite.desk.com/api/v2/customers.json?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get customers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9a712a4-8c0a-4720-ae23-03e2d802febb"
            }
          ]
        },
        {
          "id": "0317f233-23ab-4315-9620-504af1d8f76e",
          "name": "create-customer",
          "request": {
            "url": "http://yoursite.desk.com/api/v2/customers.json?format=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b86d495f-46b6-470d-b042-a1b2c82e377b"
            }
          ]
        },
        {
          "id": "e148bd25-eea9-4f53-b62e-262aa6c9bee3",
          "name": "create-customer-email",
          "request": {
            "url": {
              "protocol": "http",
              "host": "yoursite.desk.com",
              "path": [
                "api",
                "v2",
                "customers/:customer_id/emails.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "customer_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create customer email."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c21b026-3c40-4f5c-9e3d-8e945c3830d0"
            }
          ]
        }
      ]
    }
  ]
}