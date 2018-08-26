{
  "info": {
    "name": "Port+ Portdirectory API Get Companies",
    "_postman_id": "5ef1b69e-bdff-40bf-bd5a-217e683f7de2",
    "description": "Get companies where name contains input.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Companies",
      "item": [
        {
          "id": "f4f05390-2b12-44f9-a314-f2c930b93f28",
          "name": "Company_GetCompaniesOverviewContainingName",
          "request": {
            "url": "http://api.nxtport.eu/portdirectory/v1/companies?name=%7B%7D",
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
            "description": "Get companies where name contains input."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61a698c5-c712-43b3-8cd1-06dfb738ac82"
            }
          ]
        }
      ]
    }
  ]
}