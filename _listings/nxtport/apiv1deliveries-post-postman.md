{
  "info": {
    "name": "NxtPort T-mining Secure Container Release API Record delivery",
    "_postman_id": "6cac20b3-f836-4c13-9f31-dd6a6938fcbb",
    "description": "When the driver has delivered the container, a request should be sent to the server to record (create) the delivery. Note that a delivery is associated with a PickupRight, because the driver who gets a PickupRight, will automatically get a right to deliver the container. For that reason, the PickupRight must be reported.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Record",
      "item": [
        {
          "id": "fdd20b73-4539-4082-8686-c935cad4231c",
          "name": "postApiV1Deliveries",
          "request": {
            "url": "http://api.nxtport.eu/blockchain/api/v1/deliveries?api_token=%7B%7D",
            "method": "POST",
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
            "description": "When the driver has delivered the container, a request should be sent to the server to record (create) the delivery. Note that a delivery is associated with a PickupRight, because the driver who gets a PickupRight, will automatically get a right to deliver the container. For that reason, the PickupRight must be reported."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6b300f2-9c63-45e9-ab34-93bd0925b761"
            }
          ]
        }
      ]
    }
  ]
}