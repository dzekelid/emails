{
  "info": {
    "name": "AWS Simple Email Service API Delete Verified Email Address",
    "_postman_id": "6f812155-b430-45b1-b356-43d89346cbfd",
    "description": "Deletes the specified email address from the list of verified addresses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "a53e8218-c949-4232-b6c1-ce771abcf11a",
          "name": "deleteVerifiedEmailAddress",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVerifiedEmailAddress?EmailAddress=EmailAddress",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified email address from the list of verified addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90e0877c-ced4-4d91-8cc4-68a0ed61c62a"
            }
          ]
        }
      ]
    }
  ]
}