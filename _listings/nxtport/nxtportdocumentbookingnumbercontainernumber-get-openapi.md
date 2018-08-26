---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort VGM API Get VERMAS Files
  description: Returns the VERMAS files with the according booking number and container
    number
  version: 1.0.0
host: api.nxtport.eu
basePath: /VGM/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /nxtportdocument/{bookingnumber}/{containernumber}:
    get:
      summary: Get VERMAS Files
      description: Returns the VERMAS files with the according booking number and
        container number
      operationId: NxtportdocumentByBookingnumberByContainernumberGet
      x-api-path-slug: nxtportdocumentbookingnumbercontainernumber-get
      parameters:
      - in: path
        name: bookingnumber
        description: bookingnumber
      - in: path
        name: containernumber
        description: containernumber
      - in: header
        name: Ocp-Apim-Subscription-Key
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - VERMAS
      - Files
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