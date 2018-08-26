{
  "info": {
    "name": "NxtPort UN Location Codes API Get Countries",
    "_postman_id": "c8d67b9b-cc3a-46d3-9daa-8740aacf9d94",
    "description": "Get a list of all the countries. The API will return the complete list of the existing countries with their country name and 2-character country code in JSON format. The example output for a HTTP Status code 200 contains a subset of the possible outcome.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "a9a6a21c-ad40-487f-af11-d2c31a8083a6",
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
              "id": "8d453f15-879b-4a5f-87e3-7b543b7f22b0"
            }
          ]
        }
      ]
    }
  ]
}