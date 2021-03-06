---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort Big Belly API Publish Device
  description: Publish the fill level for all Big Belly devices.
  termsOfService: https://www.nxtport.eu/General-Terms-And-Conditions
  version: 1.0.0
host: api-stg.nxtport.eu
basePath: /bigbelly/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metrics:
    get:
      summary: Retrieving supported metrics
      description: "The platform allows you to retrieve supported metrics by sending
        a HTTP GET to /metrics. \nThe string-values for the attribute id can be used
        as a metricId path parameter in the City Layer operations. \nThe attribute
        granularity indicates how fine grained temporal pages should be split up when
        querying individual sources (and can be ignored here)."
      operationId: getMetrics
      x-api-path-slug: metrics-get
      responses:
        200:
          description: OK
      tags:
      - MEtrics
  /layers:
    get:
      summary: Retrieve available layers
      description: "This operation lists the currently available city layers. \nThe
        returned strings can then be used as a layerId path parameter in the /layers
        operations included in this API."
      operationId: getLayers
      x-api-path-slug: layers-get
      responses:
        200:
          description: OK
      tags:
      - Layers
  /layers/{layerId}/{metricId}/{date}:
    get:
      summary: Retrieve the city layer data for the specified layer, metric and date.
      description: 'This operation retrieves city layer data for the specified layer,
        metric and date combination. The date is passed in the following format: YYYYMMDD.
        The values for the layerId and metricId can be fetched from the /layers and
        /metrics operations.'
      operationId: getLayerDateByLayerMetricDate
      x-api-path-slug: layerslayeridmetriciddate-get
      parameters:
      - in: path
        name: date
        description: TODO
      - in: path
        name: layerId
        description: TODO
      - in: path
        name: metricId
        description: TODO
      responses:
        200:
          description: OK
      tags:
      - Layers
      - Metrics
  /layers/{layerId}/{metricId}/{date}/{hour}:
    get:
      summary: Retrieve the city layer data for the specified layer, metric and date.
      description: 'This operation retrieves city layer data for the specified layer,
        metric and date combination. The date is passed in the following format: YYYYMMDD.
        The values for the layerId and metricId can be fetched from the /layers and
        /metrics operations.'
      operationId: getLayerDateByLayerMetricDateHour
      x-api-path-slug: layerslayeridmetriciddatehour-get
      parameters:
      - in: path
        name: date
        description: TODO
      - in: path
        name: hour
        description: TODO
      - in: path
        name: layerId
        description: TODO
      - in: path
        name: metricId
        description: TODO
      responses:
        200:
          description: OK
      tags:
      - Layers
  /devices:
    post:
      summary: Publish Device
      description: Publish the fill level for all Big Belly devices.
      operationId: Publish_Devices
      x-api-path-slug: devices-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Devices
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