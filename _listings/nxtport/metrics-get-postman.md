{
  "info": {
    "name": "NxtPort Bel Air API Retrieving supported metrics",
    "_postman_id": "3b2db28d-927e-47c0-ab63-3284a60ecf00",
    "description": "The platform allows you to retrieve supported metrics by sending a HTTP GET to /metrics. \nThe string-values for the attribute id can be used as a metricId path parameter in the City Layer operations. \nThe attribute granularity indicates how fine grained temporal pages should be split up when querying individual sources (and can be ignored here).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "MEtrics",
      "item": [
        {
          "id": "6ccec4d7-c2bf-43ae-8da5-5a60d03ca0c8",
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
              "id": "4514a84f-b0c3-4925-a87a-79bebfdd3951"
            }
          ]
        }
      ]
    }
  ]
}