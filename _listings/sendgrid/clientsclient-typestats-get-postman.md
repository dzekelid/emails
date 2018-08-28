{
  "info": {
    "name": "SendGrid Get Clients Client Type Stats",
    "_postman_id": "aa08ab61-f779-4626-afc5-582ff35eb5e4",
    "description": "**This endpoint allows you to retrieve your email statistics segmented by a specific client type.**\n\n**We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.\n\n## Available Client Types\n- phone\n- tablet\n- webmail\n- desktop\n\nAdvanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "2bd627c1-5517-416e-b737-842b1a991d88",
          "name": "clients.client_type.stats.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "clients/:client_type/stats"
              ],
              "query": [
                {
                  "key": "aggregated_by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "client_type",
                  "value": "client_type",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your email statistics segmented by a specific client type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae48ae35-0147-40d8-b02a-ee14f6d25106"
            }
          ]
        }
      ]
    }
  ]
}