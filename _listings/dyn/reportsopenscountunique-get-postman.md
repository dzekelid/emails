{
  "info": {
    "name": "Dyn Retrieve Count of Email Opens",
    "_postman_id": "f3361231-4cc9-4822-8362-9b50ce74d977",
    "description": "Returns total number of unique opens for the specified account for the specified date range. Including a date range is highly recommended.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "e5f38aed-0a48-4c05-a68d-e2ad9887fddc",
          "name": "getAccounts",
          "request": {
            "url": "http://example.com/api/accounts?apikey=%7B%7D&startindex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a list of up to 25 Email Sub-Accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1e112e5-3b71-449c-91ef-ad7a2f52e5d4"
            }
          ]
        },
        {
          "id": "80b18c2e-8500-4f24-b2aa-5cd4ba2be3bd",
          "name": "getRecipientsStatus",
          "request": {
            "url": "http://example.com/api/recipients/status?apikey=%7B%7D&emailaddress=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Recipient(s) Status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "958746ee-d986-4c4f-902b-34e44014a75f"
            }
          ]
        },
        {
          "id": "06fc9e3c-b6cf-41b3-8c53-31f33b3fa2ff",
          "name": "getReportsBounces",
          "request": {
            "url": "http://example.com/api/reports/bounces?apikey=%7B%7D&bounce_code - Indicates the code associated with the bounced Email.=%7B%7D&bounce_code_id - The numeric code determined by the bounce processor.=%7B%7D&bounce_rule - Indicates the rule that caused this email to bounce.=%7B%7D&bounce_type=%7B%7D&bounce_type_id - Indicates whether the bounce type is a hard or soft bounce.nValid Values:n1 - Hard Bouncen2 - Soft Bounce=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&noheaders=%7B%7D&sender=%7B%7D&sender_id=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving the Email SPAM Complaints"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ef5ddbd-c00a-4d50-b693-3c3776c5b6b3"
            }
          ]
        },
        {
          "id": "8a346112-ddf1-414b-93f6-ab3f9b96ce75",
          "name": "getReportsBouncesCount",
          "request": {
            "url": "http://example.com/api/reports/bounces/count?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total count of Email bounces using the API requires specific syntax for the REST API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "779c7782-07ec-464a-a5b5-727fd62cf103"
            }
          ]
        },
        {
          "id": "3ffc8bcf-8ba0-444b-b78e-deed8d391bcd",
          "name": "getReportsClicksCount",
          "request": {
            "url": "http://example.com/api/reports/clicks/count?apikey=%7B%7D&domainu00a0=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total of Email links clicked"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bda1091-5a23-4501-81a1-c7f5aecd02a0"
            }
          ]
        },
        {
          "id": "490bd0a3-f402-493f-8b15-5364ed7fe57f",
          "name": "getReportsClicksCountUnique",
          "request": {
            "url": "http://example.com/api/reports/clicks/count/unique?apikey=%7B%7D&domainu00a0=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total of Email links clicked"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3c46ae7-b525-473f-b414-9463b2900a72"
            }
          ]
        },
        {
          "id": "ddbbf809-3e40-47af-9948-148c21d0d801",
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
              "id": "f7485585-d5a9-448e-91bb-4623a8dbd0f9"
            }
          ]
        },
        {
          "id": "9e7366d7-0b74-48f8-9fbc-ea23a99a9e87",
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
              "id": "b4e67902-17c1-4b3d-b835-f3d4ccf5ab1f"
            }
          ]
        },
        {
          "id": "54c68acf-d030-4890-b842-5206d23367f8",
          "name": "getReportsDelivered",
          "request": {
            "url": "http://example.com/api/reports/delivered?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Emails Delivered"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "673af7b0-4c54-41f4-b8a8-2bfd9eeada8a"
            }
          ]
        },
        {
          "id": "a42565e1-bed0-4ecf-aae9-0b5cd6f41b96",
          "name": "getReportsDeliveredCount",
          "request": {
            "url": "http://example.com/api/reports/delivered/count?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Count of Emails Delivered"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26bbf385-3c75-45fb-964b-34f82de6e794"
            }
          ]
        },
        {
          "id": "164f5897-4274-4529-83d1-2b6735f32028",
          "name": "getReportsIssues",
          "request": {
            "url": "http://example.com/api/reports/issues?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&sender_id=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Email Issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d611681d-c265-4bbc-a22a-304549a586fb"
            }
          ]
        },
        {
          "id": "1b15c9c5-6163-4dc0-8aec-084ca846f3ee",
          "name": "getReportsIssuesCount",
          "request": {
            "url": "http://example.com/api/reports/issues/count?apikey=%7B%7D&endtime=%7B%7D&starttime=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total count of Email issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35b07802-4c64-47eb-902d-b0db32b4dd66"
            }
          ]
        },
        {
          "id": "95fc912b-16a7-4519-b537-22a610d05d88",
          "name": "getReportsOpensCountUnique",
          "request": {
            "url": "http://example.com/api/reports/opens/count/unique?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns total number of unique opens for the specified account for the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ba07474-b909-4529-be52-ed60a87279d8"
            }
          ]
        }
      ]
    },
    {
      "name": "Updating.Email",
      "item": [
        {
          "id": "133a2bdc-d8ae-4aa8-8e11-24b134733432",
          "name": "putAccounts",
          "request": {
            "url": "http://example.com/api/accounts?address=%7B%7D&apikey=%7B%7D&bounceurl=%7B%7D&city=%7B%7D&companyname=%7B%7D&country=%7B%7D&generatenewapikey=%7B%7D&password=%7B%7D&phone=%7B%7D&spamurl=%7B%7D&state=%7B%7D&timezone=%7B%7D&tracklinks=%7B%7D&trackopens=%7B%7D&trackunsubscribes=%7B%7D&unsubscribeurl=%7B%7D&username=%7B%7D&zipcode=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updating an Email Sub-Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f7e08c9-d9a8-487d-8eea-ee30cb707448"
            }
          ]
        }
      ]
    },
    {
      "name": "Create.Email",
      "item": [
        {
          "id": "1d2c689e-bd77-437f-98d5-79c530c304ec",
          "name": "postAccounts",
          "request": {
            "url": "http://example.com/api/accounts?address=%7B%7D&apikey=%7B%7D&bounceurl=%7B%7D&city=%7B%7D&companyname=%7B%7D&country=%7B%7D&generatenewapikey=%7B%7D&password=%7B%7D&phone=%7B%7D&spamurl=%7B%7D&state=%7B%7D&timezone=%7B%7D&tracklinks=%7B%7D&trackopens=%7B%7D&trackunsubscribes=%7B%7D&username=%7B%7D&zipcode=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creating an Email Sub-Account using the API requires specific syntax for the REST API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "081b67f0-73ff-46ad-a06a-383b00274b06"
            }
          ]
        }
      ]
    },
    {
      "name": "Deleting.Email",
      "item": [
        {
          "id": "1a7c1729-d1b4-47fb-b96e-24b001544314",
          "name": "postAccountsDelete",
          "request": {
            "url": "http://example.com/api/accounts/delete?apikey=%7B%7D&username=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Deleting an Email Sub-Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbe94eab-305c-48d3-9046-12486c183d08"
            }
          ]
        }
      ]
    },
    {
      "name": ".Email",
      "item": [
        {
          "id": "474792d0-69b8-45da-9d03-d42197c68050",
          "name": "getOpensCount",
          "request": {
            "url": "http://example.com/api/opens/count?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns total number of opens for the specified account for the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e5062d0-839c-4d52-9907-9ae22a85c7fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Activate",
      "item": [
        {
          "id": "6ac52a91-8a21-4907-84e3-47a51c783978",
          "name": "postRecipientsActivate",
          "request": {
            "url": "http://example.com/api/recipients/activate?apikey=%7B%7D&emailaddress=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Activating a specified Recipientu2019s status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29be9c0a-28bd-4011-974d-0849376df7c5"
            }
          ]
        }
      ]
    },
    {
      "name": "Reports",
      "item": [
        {
          "id": "efab43bb-0c5f-4406-9e1f-46a5f5c251ef",
          "name": "getReportsClicks",
          "request": {
            "url": "http://example.com/api/reports/clicks?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of links clicked for the specified account during the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a53df53d-bbe8-4ad0-9401-a2ac1d86574d"
            }
          ]
        }
      ]
    },
    {
      "name": "Unique",
      "item": [
        {
          "id": "3b744cc9-2848-425d-8122-c7ec16c86770",
          "name": "getReportsClicksUnique",
          "request": {
            "url": "http://example.com/api/reports/clicks/unique?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of unique links clicked for the specified account during the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0a46f73-951e-4847-ac7c-d65989b4c09e"
            }
          ]
        }
      ]
    }
  ]
}