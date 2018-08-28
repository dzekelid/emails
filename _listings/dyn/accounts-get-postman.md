{
  "info": {
    "name": "Dyn Retrieve email sub-accounts",
    "_postman_id": "9be94fdd-3520-4b75-98a7-66787cb72547",
    "description": "Retrieving a list of up to 25 Email Sub-Accounts",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "4f988043-a200-4b5b-9074-5f5df5d5a43f",
          "name": "getAccounts",
          "request": {
            "url": "http://example.com/api/accounts?apikey=%7B%7D&startindex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a list of up to 25 Email Sub-Accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f7f2ea3-c9e6-4621-97ce-da83fd9e209f"
            }
          ]
        }
      ]
    }
  ]
}