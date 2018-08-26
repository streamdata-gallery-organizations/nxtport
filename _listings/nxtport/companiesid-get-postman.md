{
  "info": {
    "name": "Port+ Portdirectory API Get Companies",
    "_postman_id": "33eba487-290d-4521-9b3a-1f2dd135a147",
    "description": "Get a company by its id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Companies",
      "item": [
        {
          "id": "03d9b3c8-d6c4-4c73-a5ae-e0507b068ec9",
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
              "id": "b8238282-a72d-46a4-ba24-2fc2ee9e2157"
            }
          ]
        },
        {
          "id": "b62d27fc-f1d3-44a7-a1e4-788fca277489",
          "name": "Company_GetCompanyById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "portdirectory",
                "v1",
                "companies/:id"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Get a company by its id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "baad334d-1ba8-4ba9-be81-32aa6ffb9fd5"
            }
          ]
        }
      ]
    }
  ]
}