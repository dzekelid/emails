{
  "info": {
    "name": "SendGrid Get Clients Stats",
    "_postman_id": "8d06e36a-eebb-4f44-b5d3-162648f8e336",
    "description": "**This endpoint allows you to retrieve your email statistics segmented by client type.**\n\n**We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.\n\nAdvanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "d0f957ce-7232-43f7-bfe6-7e0970708794",
          "name": "clients.stats.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/clients/stats?aggregated_by=%7B%7D&end_date=%7B%7D&No Name=%7B%7D&start_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your email statistics segmented by client type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acb857f5-2584-4b20-bbdf-a0bd58d807d0"
            }
          ]
        }
      ]
    }
  ]
}