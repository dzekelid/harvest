---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Get Harvest Backends
  description: List all available harvest backends
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /harvest/backends:
    get:
      summary: Get Harvest Backends
      description: List all available harvest backends
      operationId: getHarvestBackends
      x-api-path-slug: harvestbackends-get
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Backends
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