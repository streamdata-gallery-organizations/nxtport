---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort Bel Air API Retrieving supported metrics
  description: "The platform allows you to retrieve supported metrics by sending a
    HTTP GET to /metrics. \nThe string-values for the attribute id can be used as
    a metricId path parameter in the City Layer operations. \nThe attribute granularity
    indicates how fine grained temporal pages should be split up when querying individual
    sources (and can be ignored here)."
  termsOfService: https://www.nxtport.eu/General-Terms-And-Conditions
  version: 1.0.0
host: api-stg.nxtport.eu
basePath: /belair/v1
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