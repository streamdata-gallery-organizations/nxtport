---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
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
  /vessels/in-port:
    get:
      summary: Get Vessels In Port
      description: Get all the in-port vessels of BEANR and BEZEE
      operationId: Vessels_InPort
      x-api-path-slug: vesselsinport-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Vesses
      - Ports
---