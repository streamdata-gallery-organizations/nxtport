{
  "info": {
    "name": "NxtPort UN Location Codes API Get Locations",
    "_postman_id": "ac1a8187-9036-4986-a69c-58ad8e6583ea",
    "description": "This api will return a (paged) list of locations that match the search parameters (query parameters) ordered by the name without diacritics.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Locations",
      "item": [
        {
          "id": "15ccf0b5-db91-45a4-8ebd-a67ea44d48f6",
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
              "id": "a8517b85-0620-488c-9edf-39d54ea0537f"
            }
          ]
        }
      ]
    }
  ]
}