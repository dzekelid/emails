{
  "info": {
    "name": "Dyn Retrieve Count of Email SPAM Complaints",
    "_postman_id": "020ce324-b37d-4175-ac88-4bd1be640c07",
    "description": "Retrieving a total count of Email complaints",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "d81acb22-8aae-4b04-9434-d4e82b171a2d",
          "name": "getReportsComplaints",
          "request": {
            "url": "http://example.com/api/reports/complaints?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Email SPAM Complaints"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38ad8399-9d22-43a9-a22a-43b1581fa4a0"
            }
          ]
        },
        {
          "id": "868ecbe0-fb94-4bb1-bdc1-1671dfbb8843",
          "name": "getReportsComplaintsCount",
          "request": {
            "url": "http://example.com/api/reports/complaints/count?apikey=%7B%7D&endtime=%7B%7D&starttime=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total count of Email complaints"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17e9cbf4-3ae4-4b6a-aaf2-60c91d5d7f8e"
            }
          ]
        }
      ]
    }
  ]
}