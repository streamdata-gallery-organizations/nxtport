---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: Portcall+ API Get Expected Vessels
  description: Get all the expected vessels of BEANR and BEZEE
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /vessels/expected:
    get:
      summary: Get Expected Vessels
      description: Get all the expected vessels of BEANR and BEZEE
      operationId: Vessels_Expected
      x-api-path-slug: vesselsexpected-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Vessels
      - Ports
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