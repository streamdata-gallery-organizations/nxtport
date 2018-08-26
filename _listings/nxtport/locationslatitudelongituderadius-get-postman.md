{
  "info": {
    "name": "NxtPort UN Location Codes API Get Locations Latitude Longitude Radius",
    "_postman_id": "cbfc75d5-0d5d-438b-bf3a-e668aac1daee",
    "description": "This api will return locations in a certain radius of a point, ordered by distance , not necessarily in the same country",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Locations",
      "item": [
        {
          "id": "38ca6444-13d8-401b-b3f9-d29f00af3b3d",
          "name": "searchLocations",
          "request": {
            "url": "http://api.nxtport.eu/unlocodes/v1/locations?code=%7B%7D&country=%7B%7D&page=%7B%7D&searchterm=%7B%7D&size=%7B%7D&subdiv=%7B%7D",
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
            "description": "This api will return a (paged) list of locations that match the search parameters (query parameters) ordered by the name without diacritics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7da9dc0-a6e8-4072-a88b-c3b9b7819820"
            }
          ]
        },
        {
          "id": "32539ad4-db9d-4cde-8f9d-220192c8c0bf",
          "name": "locations_getinNeighbourhood",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "unlocodes",
                "v1",
                "locations/:latitude/:longitude/:radius"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "size",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "latitude",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "longitude",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "radius",
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
            "description": "This api will return locations in a certain radius of a point, ordered by distance , not necessarily in the same country"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e9b3fe4-957c-4d00-a9bf-fdcdd22e46df"
            }
          ]
        }
      ]
    }
  ]
}