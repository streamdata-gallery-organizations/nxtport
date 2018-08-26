{
  "info": {
    "name": "NxtPort Bel Air API Retrieve available layers",
    "_postman_id": "691ef98d-54e7-4367-b913-a2f0582540ae",
    "description": "This operation lists the currently available city layers. \nThe returned strings can then be used as a layerId path parameter in the /layers operations included in this API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "MEtrics",
      "item": [
        {
          "id": "e9b298cc-e244-4994-963c-fb9be0aaa68e",
          "name": "getMetrics",
          "request": {
            "url": "http://api-stg.nxtport.eu/belair/v1/metrics",
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
            "description": "The platform allows you to retrieve supported metrics by sending a HTTP GET to /metrics. \nThe string-values for the attribute id can be used as a metricId path parameter in the City Layer operations. \nThe attribute granularity indicates how fine grained temporal pages should be split up when querying individual sources (and can be ignored here)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09d539be-bfd2-4774-bef1-c162d29b6c82"
            }
          ]
        }
      ]
    },
    {
      "name": "Layers",
      "item": [
        {
          "id": "0532298d-00c2-4d37-baee-29362a780446",
          "name": "getLayers",
          "request": {
            "url": "http://api-stg.nxtport.eu/belair/v1/layers",
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
            "description": "This operation lists the currently available city layers. \nThe returned strings can then be used as a layerId path parameter in the /layers operations included in this API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7eae114e-c640-4fff-bf6d-9dfbb8a05a0b"
            }
          ]
        }
      ]
    }
  ]
}