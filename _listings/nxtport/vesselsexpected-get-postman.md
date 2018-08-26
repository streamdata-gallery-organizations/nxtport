{
  "info": {
    "name": "Portcall+ API Get Expected Vessels",
    "_postman_id": "9b7583d3-f75b-4348-a965-602a38835aff",
    "description": "Get all the expected vessels of BEANR and BEZEE",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shipping",
      "item": [
        {
          "id": "f1ed5eee-b8e3-422c-88a1-7273466e59de",
          "name": "Vessels_Expected",
          "request": {
            "url": "http://api-sb.nxtport.eu/PortCallPlus/v1/vessels/expected",
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
            "description": "Get all the expected vessels of BEANR and BEZEE"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dac18b3d-a8f2-4263-8bf6-af79a33d0f7a"
            }
          ]
        }
      ]
    }
  ]
}