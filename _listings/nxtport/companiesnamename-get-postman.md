{
  "info": {
    "name": "Port+ Portdirectory API Get Companies Name Name",
    "_postman_id": "a50b2471-e2d3-4259-a5ec-523c270952a8",
    "description": "Get a company by its name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Companies",
      "item": [
        {
          "id": "0a4c1c16-4f68-4a2b-bfa4-606fee6a67eb",
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
              "id": "67adeb3f-af8e-40e9-ba4c-318bc5e24d37"
            }
          ]
        },
        {
          "id": "22400e60-9802-4e24-bb72-4b32c10672f2",
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
              "id": "1b440ce8-77fb-4bb1-9341-a87285d28731"
            }
          ]
        },
        {
          "id": "26c1474a-ff91-4ae5-8baf-1ad062fb64cd",
          "name": "Company_GetCompanyByName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "portdirectory",
                "v1",
                "companies/name/:name"
              ],
              "variable": [
                {
                  "id": "name",
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
            "description": "Get a company by its name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b923cd16-e7cc-4ad7-a43f-59b3ad50be23"
            }
          ]
        }
      ]
    }
  ]
}