{
  "info": {
    "name": "Dezrez Gets Email Sync Security Credentials",
    "_postman_id": "ecac8182-657c-43d5-a775-19199b84089a",
    "description": "Gets email sync security credentials.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Security",
      "item": [
        {
          "id": "4b91d094-5bce-491e-a929-07614bf1906f",
          "name": "Credentials_DeleteUsernamePasswordByname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/credentials/deleteusernamepassword/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Delete security credentials."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a9d5080-ac54-4906-8e56-664dbe627b61"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "4b782ca6-1c9b-4330-bb17-944345770eca",
          "name": "Credentials_EmailSyncUsernamePasswordBycredentialDataContract.usernameBycredentialDataContract.passw",
          "request": {
            "url": "http://api.dezrez.com/api/credentials/emailsync/usernamepassword?credentialDataContract.password=%7B%7D&credentialDataContract.username=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Gets email sync security credentials."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6267abf-b609-46ef-aba9-6a4a0d37abfd"
            }
          ]
        }
      ]
    }
  ]
}