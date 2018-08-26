{
  "info": {
    "name": "NxtPort T-mining Secure Container Release API List Containers",
    "_postman_id": "d345bfbd-d082-45c3-b92e-2ed32e1ea1a9",
    "description": "Get all containers currently in the database. Only Containers accessible by the user will be reported.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "2102dd52-67cf-48db-bca7-b68d9b563883",
          "name": "getApiV1Containers",
          "request": {
            "url": "http://api.nxtport.eu/blockchain/api/v1/containers?api_token=%7B%7D",
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
            "description": "Get all containers currently in the database. Only Containers accessible by the user will be reported."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71da1244-c921-4278-a37b-0cc40fce5d49"
            }
          ]
        }
      ]
    }
  ]
}