{
  "info": {
    "name": "NxtPort T-mining Secure Container Release API Block",
    "_postman_id": "0e84a2d3-ee11-41d3-b74b-bd7998573c20",
    "description": "Blocking a release is done by a delete. This will revoke the PickupRight from the consignee. The Container and its PickupRight are deleted. Afterwards it is still possible to release again.\n The following conditions apply for this to work:\n* the container must have been released, i.e. there must be a vallid PickupRight   for the Container\n* the PickupRight should not be transferred to another Organization than the one that got the relesase initially\n* the PickupRight should not yet be assigned (to a driver / skipper)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Block",
      "item": [
        {
          "id": "98901722-2e11-4553-9b77-d13cad2be41d",
          "name": "deleteApiV1Releases",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "blockchain",
                "api/v1/releases/:id"
              ],
              "query": [
                {
                  "key": "api_token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Blocking a release is done by a delete. This will revoke the PickupRight from the consignee. The Container and its PickupRight are deleted. Afterwards it is still possible to release again.\n The following conditions apply for this to work:\n* the container must have been released, i.e. there must be a vallid PickupRight   for the Container\n* the PickupRight should not be transferred to another Organization than the one that got the relesase initially\n* the PickupRight should not yet be assigned (to a driver / skipper)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e12ef6e-899a-418d-a6e1-cdda505094b8"
            }
          ]
        }
      ]
    }
  ]
}