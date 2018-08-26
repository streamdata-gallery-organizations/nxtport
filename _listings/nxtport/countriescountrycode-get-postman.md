{
  "info": {
    "name": "NxtPort UN Location Codes API Get Countries Countrycode",
    "_postman_id": "488d8d23-d88b-4b53-9e4d-3b74bccf243b",
    "description": "Get the details of 1 specific country, specified by the country code in the query parameter. Both the country name and country code are returned in a JSON object. The example response in case of HTTP Status Code 200 contains the result when requested for countryCode BE.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "1c37746e-1f50-4a7a-94da-2fc31165a5d3",
          "name": "getCountries",
          "request": {
            "url": "http://api.nxtport.eu/unlocodes/v1/countries",
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
            "description": "Get a list of all the countries. The API will return the complete list of the existing countries with their country name and 2-character country code in JSON format. The example output for a HTTP Status code 200 contains a subset of the possible outcome."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c93a30b9-ca86-4225-9b03-5c62ecca4075"
            }
          ]
        },
        {
          "id": "78078dcb-0e94-49e8-b4d2-c37522d61082",
          "name": "getCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "unlocodes",
                "v1",
                "countries/:countryCode"
              ],
              "variable": [
                {
                  "id": "countryCode",
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
            "description": "Get the details of 1 specific country, specified by the country code in the query parameter. Both the country name and country code are returned in a JSON object. The example response in case of HTTP Status Code 200 contains the result when requested for countryCode BE."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "872169c1-56ab-4ad9-a506-8dffd6a2fdd6"
            }
          ]
        },
        {
          "id": "d67cdb7c-79d1-409f-b59d-139433f367e9",
          "name": "getCountrySubdivisions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "unlocodes",
                "v1",
                "countries/:countryCode/subdivisions"
              ],
              "variable": [
                {
                  "id": "countryCode",
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
            "description": "Get a list of all the subdivisions of a certain country, specified by the country code in the query parameter. The example response contains a subset of the output when requested for BE."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "189d5cbf-cd26-4eea-a0d1-a895e3e32811"
            }
          ]
        },
        {
          "id": "d4fc6a98-a466-4f21-bf50-8486448e4a8c",
          "name": "getCountrySubdivision",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "unlocodes",
                "v1",
                "countries/:countryCode/subdivisions/:subdivisionCode"
              ],
              "variable": [
                {
                  "id": "countryCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subdivisionCode",
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
            "description": "Get the details of 1 specific subdivision, based on the countryCode and subdivisionCode in the query parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f56a21a8-6b74-48ac-a53a-c8928ffdb608"
            }
          ]
        }
      ]
    }
  ]
}