{
  "info": {
    "name": "NxtPort T-mining Secure Container Release API Get container events",
    "_postman_id": "f33012c1-160c-4ee4-b81c-c0cd108e9561",
    "description": "Get the list of Events related to a container",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Container",
      "item": [
        {
          "id": "502d25fb-20d4-4da8-8bf8-2bdbb160aba2",
          "name": "getApiV1ContainersEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "blockchain",
                "api/v1/containers/:id/events"
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
            "description": "Get the list of Events related to a container"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd6d7e1d-7961-4326-9eaa-8f9646f9cd0c"
            }
          ]
        }
      ]
    }
  ]
}