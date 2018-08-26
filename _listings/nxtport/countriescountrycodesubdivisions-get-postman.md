{
  "info": {
    "name": "NxtPort UN Location Codes API Get Countries Code Subdivisions",
    "_postman_id": "0b86584d-6399-4621-9c6e-bce7823f290d",
    "description": "Get a list of all the subdivisions of a certain country, specified by the country code in the query parameter. The example response contains a subset of the output when requested for BE.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "34b9a02a-eabb-4d3b-a49e-b14229ea313d",
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
              "id": "21ded4c0-5e9e-4695-a601-8f7fdf6b7187"
            }
          ]
        },
        {
          "id": "79e0d4d5-3ef6-4963-8d14-1eaa61da9436",
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
              "id": "70b9f994-4864-4e22-a6e6-ce28507fff07"
            }
          ]
        },
        {
          "id": "6ec0ae75-d521-4c6d-9f6a-241da67927a1",
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
              "id": "0b55f796-2f30-4e3a-b732-f83980a3a18e"
            }
          ]
        },
        {
          "id": "7cc13227-d137-474e-845b-0650affae123",
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
              "id": "d94f3970-a6d4-49ab-83c8-b0a05988669e"
            }
          ]
        }
      ]
    }
  ]
}