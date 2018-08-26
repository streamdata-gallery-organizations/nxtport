{
  "info": {
    "name": "NxtPort T-mining Secure Container Release API List",
    "_postman_id": "a1b79ccc-da1f-4778-be74-627359bea6f1",
    "description": "List all Locations with their details. Locations have a type, name and the ISRS Locode.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "01b1d5a5-b398-4870-920b-abe65dcab35e",
          "name": "getApiV1Locations",
          "request": {
            "url": "http://api.nxtport.eu/blockchain/api/v1/locations?api_token=%7B%7D",
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
            "description": "List all Locations with their details. Locations have a type, name and the ISRS Locode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "448a8ff9-8945-43e2-bf63-40cdc85a6158"
            }
          ]
        }
      ]
    }
  ]
}