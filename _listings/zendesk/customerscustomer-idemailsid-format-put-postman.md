{
  "info": {
    "name": "Sales Force Desk API Update Customer Email",
    "_postman_id": "4a8dd65b-b740-4773-9ae3-9961be3764c5",
    "description": "Update customer email.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Customers",
      "item": [
        {
          "id": "7125bc16-f21e-4b4a-9232-2a436d527c39",
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
              "id": "88512091-1947-43a0-8e2d-55b2a7ecaad2"
            }
          ]
        },
        {
          "id": "eae6ccbc-fa0a-4af5-abc9-7a55714acaf6",
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
              "id": "d20ecfb5-e4d7-4a6a-b236-e70d36f7e74a"
            }
          ]
        },
        {
          "id": "a3af325d-acac-4e5c-81ff-b9e4e6e16572",
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
              "id": "b77559fe-3a07-4705-bdaf-826f72f65168"
            }
          ]
        },
        {
          "id": "037a5724-89a7-4702-a82b-6b31df3477ed",
          "name": "update-customer-email",
          "request": {
            "url": {
              "protocol": "http",
              "host": "yoursite.desk.com",
              "path": [
                "api",
                "v2",
                "customers/:customer_id/emails/:id.json"
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
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update customer email."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38a137f6-7e6e-4ca9-91ad-f751583ae383"
            }
          ]
        }
      ]
    }
  ]
}