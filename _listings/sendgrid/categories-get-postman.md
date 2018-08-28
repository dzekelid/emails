{
  "info": {
    "name": "SendGrid Get Categories",
    "_postman_id": "745ff1fc-fc78-4f88-8fb7-208918b7920b",
    "description": "**This endpoint allows you to retrieve a list of all of your categories.**\n\nCategories can help organize your email analytics by enabling you to ???tag??? emails by type or broad topic. You can define your own custom categories. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "778f97ae-40d6-4851-af7e-f6dbbdbcd2bb",
          "name": "GET_categories",
          "request": {
            "url": "http://api.sendgrid.com/v3/categories?category=%7B%7D&limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a list of all of your categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ee6a1f7-6edb-43ae-b8e4-e47f90db9a3a"
            }
          ]
        }
      ]
    }
  ]
}