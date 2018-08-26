---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort UN Location Codes API Get Countries Country Code Subdivisions Code
  description: Get the details of 1 specific subdivision, based on the countryCode
    and subdivisionCode in the query parameters.
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
  /countries/{countryCode}:
    get:
      summary: Get Countries Countrycode
      description: Get the details of 1 specific country, specified by the country
        code in the query parameter. Both the country name and country code are returned
        in a JSON object. The example response in case of HTTP Status Code 200 contains
        the result when requested for countryCode BE.
      operationId: getCountry
      x-api-path-slug: countriescountrycode-get
      parameters:
      - in: path
        name: countryCode
        description: 2-character country code
      responses:
        200:
          description: OK
      tags:
      - Countries
      - Countrycode
  /countries/{countryCode}/subdivisions:
    get:
      summary: Get Countries Code Subdivisions
      description: Get a list of all the subdivisions of a certain country, specified
        by the country code in the query parameter. The example response contains
        a subset of the output when requested for BE.
      operationId: getCountrySubdivisions
      x-api-path-slug: countriescountrycodesubdivisions-get
      parameters:
      - in: path
        name: countryCode
        description: 2-character country code
      responses:
        200:
          description: OK
      tags:
      - Countries
      - Countrycode
      - Subdivisions
  /countries/{countryCode}/subdivisions/{subdivisionCode}:
    get:
      summary: Get Countries Country Code Subdivisions Code
      description: Get the details of 1 specific subdivision, based on the countryCode
        and subdivisionCode in the query parameters.
      operationId: getCountrySubdivision
      x-api-path-slug: countriescountrycodesubdivisionssubdivisioncode-get
      parameters:
      - in: path
        name: countryCode
        description: 2-character country code
      - in: path
        name: subdivisionCode
        description: 3-character subdivision code
      responses:
        200:
          description: OK
      tags:
      - Countries
      - Countrycode
      - Subdivisions
      - Subdivisioncode
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