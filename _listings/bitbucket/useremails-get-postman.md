{
  "info": {
    "name": "Bitbucket Get User Emails",
    "_postman_id": "ad31b6b3-33bb-4c82-9a67-4f813be5f612",
    "description": "Returns all the authenticated user's email addresses. Both\nconfirmed and unconfirmed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "8f8a0835-3340-4bae-9d0c-e8638f82234f",
          "name": "getUserEmails",
          "request": {
            "url": "http://api.bitbucket.org/2.0/user/emails",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all the authenticated user's email addresses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19bf8934-dd29-4a65-87b4-42add64e338b"
            }
          ]
        }
      ]
    }
  ]
}