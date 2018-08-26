{
  "info": {
    "name": "NxtPort Consignment API Returns the file with corresponding blnumbers and containernumber.",
    "_postman_id": "fab0a703-ba67-46ee-9c94-fb99f5fbca92",
    "description": "Returns the file with corresponding blnumbers and containernumber..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "9284bf6a-6774-4431-bab0-b1091a35d469",
          "name": "NxtportdocumentByBlnumberSnByStayNumberGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "Consignment",
                "v1",
                "nxtportdocument/:blnumber/sn/:stayNumber"
              ],
              "variable": [
                {
                  "id": "blnumber",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "stayNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Ocp-Apim-Subscription-Key",
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
            "description": "Returns the file with corresponding blnumbers and staynumber.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b5b476e-ac1d-4d2b-85f0-9b69e379b609"
            }
          ]
        },
        {
          "id": "34e20f3b-2f12-408e-aad1-ed7c692b0653",
          "name": "NxtportdocumentByBlnumberCnByContainerNumberGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "Consignment",
                "v1",
                "nxtportdocument/:blnumber/cn/:containerNumber"
              ],
              "variable": [
                {
                  "id": "blnumber",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "containerNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Ocp-Apim-Subscription-Key",
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
            "description": "Returns the file with corresponding blnumbers and containernumber.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d46ae9a-6779-4cc0-bda7-091823f2bf89"
            }
          ]
        }
      ]
    }
  ]
}