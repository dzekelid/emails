{
  "info": {
    "name": "SendGrid Get Ips Pools Pool Name",
    "_postman_id": "251efb2b-6911-4e70-a0b3-2c130c19bcb0",
    "description": "**This endpoint allows you to list all of the IP addresses that are in a specific IP pool.**\n\nIP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.\n\nIP pools can only be used with whitelabeled IP addresses.\n\nIf an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "902a8e1a-7f3e-45a8-8415-27dd49b74518",
          "name": "ips.pools.pool_name.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "ips/pools/:pool_name"
              ],
              "variable": [
                {
                  "id": "pool_name",
                  "value": "pool_name",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to list all of the IP addresses that are in a specific IP pool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61acee2f-28e8-4ad9-b3df-fa8f619b15bd"
            }
          ]
        }
      ]
    }
  ]
}