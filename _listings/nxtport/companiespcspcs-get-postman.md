{
  "info": {
    "name": "Port+ Portdirectory API Get Companies Pcs Pcs",
    "_postman_id": "529888e5-b745-4397-b93a-59ded9cbaf8d",
    "description": "Get a company by its pcs code.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Companies",
      "item": [
        {
          "id": "75322a69-878e-4bac-8f4b-880dfaa55c30",
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
              "id": "5d6b5718-cbad-4382-9ac4-3b6aa9479f5e"
            }
          ]
        },
        {
          "id": "d54f04ca-c8fc-4f63-8974-370a20c0a599",
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
              "id": "ea575611-6167-4742-8141-c7dfd1bebd0e"
            }
          ]
        },
        {
          "id": "d4ccc154-91a1-4f1e-8829-1e7af707af94",
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
              "id": "e5483b0d-74e1-4907-80af-9b22a9a56d80"
            }
          ]
        },
        {
          "id": "8a4df8f5-2f58-4ac8-9304-49e53f7ded0d",
          "name": "Company_GetCompanyByPcs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "portdirectory",
                "v1",
                "companies/pcs/:pcs"
              ],
              "variable": [
                {
                  "id": "pcs",
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
            "description": "Get a company by its pcs code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c941bb85-4ded-4f11-87ac-41f3bd785540"
            }
          ]
        }
      ]
    }
  ]
}