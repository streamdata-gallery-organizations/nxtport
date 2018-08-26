---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort UN Location Codes API Get Countries
  description: Get a list of all the countries. The API will return the complete list
    of the existing countries with their country name and 2-character country code
    in JSON format. The example output for a HTTP Status code 200 contains a subset
    of the possible outcome.
  version: 1.0.0
host: api.nxtport.eu
basePath: /unlocodes/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /countries:
    get:
      summary: Get Countries
      description: Get a list of all the countries. The API will return the complete
        list of the existing countries with their country name and 2-character country
        code in JSON format. The example output for a HTTP Status code 200 contains
        a subset of the possible outcome.
      operationId: getCountries
      x-api-path-slug: countries-get
      responses:
        200:
          description: OK
      tags:
      - Countries
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---