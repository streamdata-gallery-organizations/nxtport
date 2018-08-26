{
  "info": {
    "name": "NxtPort UN Location Codes API Get Countries Country Code Subdivisions Code",
    "_postman_id": "2d41f18a-dcc7-4187-a440-03956e49269b",
    "description": "Get the details of 1 specific subdivision, based on the countryCode and subdivisionCode in the query parameters.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "562f9134-06d2-4222-a5c7-42a2fd318c12",
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
              "id": "ab5df6e0-17e0-4fcb-86bd-0f8f87b1625d"
            }
          ]
        },
        {
          "id": "346a8e8a-e0b2-41bf-a0de-02edfdccefcd",
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
              "id": "d6a29d1f-82ff-496b-9964-e9128bb7bbdc"
            }
          ]
        },
        {
          "id": "2c1b3188-0961-4a6c-b346-4ceb7d81cb07",
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
              "id": "4c5c6b37-a3e8-4347-abc8-6c0230a1e0cd"
            }
          ]
        },
        {
          "id": "97fb4b17-b2ac-46e4-afaa-a3a8e2d8e0be",
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
              "id": "3fdb7c7c-c8e4-4bbc-a1ec-2e02e0f9c217"
            }
          ]
        }
      ]
    }
  ]
}