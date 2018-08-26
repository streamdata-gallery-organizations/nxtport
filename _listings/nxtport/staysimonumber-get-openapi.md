---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort Vessel Stay API Get Stay
  description: Get a single stay by IMO number.
  version: 1.0.0
host: api.nxtport.eu
basePath: /sa/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stays/{imoNumber}:
    get:
      summary: Get Stay
      description: Get a single stay by IMO number.
      operationId: Stays By ImoNumber
      x-api-path-slug: staysimonumber-get
      parameters:
      - in: path
        name: imoNumber
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Stays
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