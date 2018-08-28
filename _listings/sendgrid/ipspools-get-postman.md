{
  "info": {
    "name": "SendGrid Get Ips Pools",
    "_postman_id": "24623408-6d7a-48ad-8dd1-fcc064cb8977",
    "description": "**This endpoint allows you to retreive all of your IP pools.**\n\nIP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.\n\nIP pools can only be used with whitelabeled IP addresses.\n\nIf an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "e372f2b4-5e0a-4684-96d3-76f1c15cffbf",
          "name": "ips.pools.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/ips/pools",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retreive all of your IP pools"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5bfe103-b35b-4f95-85da-1c7db277e863"
            }
          ]
        }
      ]
    }
  ]
}