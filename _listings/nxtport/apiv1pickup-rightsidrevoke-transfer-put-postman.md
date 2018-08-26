{
  "info": {
    "name": "NxtPort T-mining Secure Container Release API Revoke Transfer",
    "_postman_id": "470b73e3-c286-4b8c-a163-3273aeed4275",
    "description": "Revoke the current PickupRight transfer. This must be used in case you did a transfer of a PickupRight to another Organization and you want to cancel this. This action is only possible as long as the PickupRight is not assigned.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Revoke",
      "item": [
        {
          "id": "32718e90-881b-493a-b07b-4930bd4df5bb",
          "name": "putApiV1PickupRightsRevokeAssignment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "blockchain",
                "api/v1/pickup_rights/:id/revoke_assignment"
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
            "method": "PUT",
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
            "description": "Revoke the current PickupRight assignment. This must be used in case you did an assign of a PickupRight to a driver and you want to cancel this. This action is only possible as long as the PickupRight is not exercised."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30e307ac-87c0-4d72-ae94-c5dd292ab424"
            }
          ]
        },
        {
          "id": "17eddbb7-6d92-40aa-98d9-b4b974f40f5d",
          "name": "putApiV1PickupRightsRevokeTransfer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "blockchain",
                "api/v1/pickup_rights/:id/revoke_transfer"
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
            "method": "PUT",
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
            "description": "Revoke the current PickupRight transfer. This must be used in case you did a transfer of a PickupRight to another Organization and you want to cancel this. This action is only possible as long as the PickupRight is not assigned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5723093e-df26-4928-9a57-a1ed2aa6b183"
            }
          ]
        }
      ]
    }
  ]
}