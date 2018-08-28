{
  "info": {
    "name": "Dyn Retrieve Email SPAM Complaints",
    "_postman_id": "0ce1520b-4175-4386-be35-d9a14ba6a3ef",
    "description": "Retrieve Email SPAM Complaints",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "a634205b-57c0-4e04-979c-6e998b04a0e1",
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
              "id": "1f172807-a969-4ff7-adda-67c001565d1f"
            }
          ]
        }
      ]
    }
  ]
}