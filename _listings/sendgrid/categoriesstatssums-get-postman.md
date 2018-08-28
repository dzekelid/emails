{
  "info": {
    "name": "SendGrid Get Categories Stats Sums",
    "_postman_id": "4ac5925b-dca4-4433-8d0f-fe658e17a71f",
    "description": "**This endpoint allows you to retrieve the total sum of each email statistic for every category over the given date range.**\n\nIf you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.\n\nCategories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "af325034-e06e-44f4-b36c-5eb476eac540",
          "name": "categories.stats.sums.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/categories/stats/sums?aggregated_by=%7B%7D&end_date=%7B%7D&limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D&sort_by_direction=%7B%7D&sort_by_metric=%7B%7D&start_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve the total sum of each email statistic for every category over the given date range"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d405b12-53a7-492b-95d7-25bdcb8f4407"
            }
          ]
        }
      ]
    }
  ]
}