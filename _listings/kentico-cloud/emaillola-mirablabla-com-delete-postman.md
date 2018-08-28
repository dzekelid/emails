{
  "info": {
    "name": "Kentico Cloud Delete data of visitor by email",
    "_postman_id": "2bdc0914-6d21-4dff-99f0-986a042de695",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "3788de40-e946-43ec-a429-60bed565886d",
          "name": "Segment569030c752a544f5A243C5285b3eb24eVisitorsBySegmentNameGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "deliver.kenticocloud.com",
              "path": [
                "segment/569030c7-52a5-44f5-a243-c5285b3eb24e/:SegmentName/visitors"
              ],
              "variable": [
                {
                  "id": "SegmentName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve visitors that match the specified segment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86fdeb33-e2fc-4a6d-982a-24f6cfb03162"
            }
          ]
        },
        {
          "id": "5f7c24ac-af29-46ea-9e3a-70647858272f",
          "name": "Visitor569030c752a544f5A243C5285b3eb24e7888c9a3824a11f1SegmentsGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/7888c9a3824a11f1/segments",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the names of segments that the specified visitor belongs to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7260c7f1-324e-466b-bf0f-98eeb8f05833"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieving",
      "item": [
        {
          "id": "8ab0f1ac-bf98-4576-a85d-eb73c1dfa165",
          "name": "Visitor569030c752a544f5A243C5285b3eb24eE3e9e191a12b9257SegmentGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/e3e9e191a12b9257/segment",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use the Personalization API to retrieve the list of segments that the specified visitor belongs to.\n\n* Authenticate the request using your Personalization API Key.\n* Specify the User ID of the visitor you are asking about.\n \nSee <https://developer.kenticocloud.com/docs/personalizing-content#section-retrieving-visitor-s-segments> for more details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ebb7de2-1dbc-4600-90f8-3b75d3362140"
            }
          ]
        }
      ]
    },
    {
      "name": "View",
      "item": [
        {
          "id": "63ea2c52-3113-4cb6-a403-8804799e67c8",
          "name": "Uid7888c9a3824a11f1Get",
          "request": {
            "url": "http://deliver.kenticocloud.com/uid/7888c9a3824a11f1",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "View data of visitor by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dc8150b-e2ef-445a-88a2-1dc22f5d677a"
            }
          ]
        },
        {
          "id": "29632d3a-8f40-4827-b99d-19feb3c40f56",
          "name": "EmailLolaMiraBlablaComGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/email/lola.mira@blabla.com",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "View data of visitor by email"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02db2d4e-364a-4dd8-a6c5-a4c40552f4bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Data",
      "item": [
        {
          "id": "21296ee7-2ff1-4444-9204-686d29ef70f8",
          "name": "Uid7888c9a3824a11f1Delete",
          "request": {
            "url": "http://deliver.kenticocloud.com/uid/7888c9a3824a11f1",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete data of visitor by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "279c306a-feca-47ae-99f8-2c6970a602ab"
            }
          ]
        },
        {
          "id": "99dd9de8-8ef5-4cf8-9eb0-00499874f33c",
          "name": "EmailLolaMiraBlablaComDelete",
          "request": {
            "url": "http://deliver.kenticocloud.com/email/lola.mira@blabla.com",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete data of visitor by email"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95de1d01-0e5f-450a-a35a-ae13d7ab4e92"
            }
          ]
        }
      ]
    }
  ]
}