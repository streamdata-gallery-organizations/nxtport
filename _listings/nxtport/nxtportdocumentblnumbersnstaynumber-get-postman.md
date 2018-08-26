{
  "info": {
    "name": "NxtPort Consignment API Returns the file with corresponding blnumbers and staynumber.",
    "_postman_id": "688175d9-c5e6-4cb0-b182-928ce4d82219",
    "description": "Returns the file with corresponding blnumbers and staynumber..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "ef84bcfd-dbb8-4631-9bff-34cf702d9b28",
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
              "id": "a8555287-5f1d-452b-851d-d0df6e87b468"
            }
          ]
        }
      ]
    }
  ]
}