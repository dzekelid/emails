{
  "info": {
    "name": "SendGrid Get Browsers Stats",
    "_postman_id": "0152b3ab-8a32-4a1c-a0aa-31d581d993c1",
    "description": "**This endpoint allows you to retrieve your email statistics segmented by browser type.**\n\n**We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.\n\nAdvanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "48075d8d-f348-427d-bf6c-462bd4028946",
          "name": "browsers.stats.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/browsers/stats?aggregated_by=%7B%7D&browsers=%7B%7D&end_date=%7B%7D&limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D&start_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your email statistics segmented by browser type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "784cc392-238f-4a1c-b862-b091b95e9f79"
            }
          ]
        }
      ]
    }
  ]
}