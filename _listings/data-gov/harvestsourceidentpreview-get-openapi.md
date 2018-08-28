---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Get Harvest Source Ent Preview
  description: Preview a single harvest source given an ID or a slug
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
  /harvest/job/{ident}/:
    get:
      summary: Get Harvest Job
      description: List all jobs for a given source
      operationId: getHarvestJobEnt
      x-api-path-slug: harvestjobident-get
      parameters:
      - in: path
        name: ident
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Job
      - Ent
  /harvest/job_status:
    get:
      summary: Get Harvest Job Status
      description: List all available harvesters
      operationId: getHarvestJobStatus
      x-api-path-slug: harvestjob-status-get
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Job
      - Status
  /harvest/source/{ident}:
    delete:
      summary: Delete Harvest Source Ent
      description: ""
      operationId: deleteHarvestSourceEnt
      x-api-path-slug: harvestsourceident-delete
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
    get:
      summary: Get Harvest Source Ent
      description: Get a single source given an ID or a slug
      operationId: getHarvestSourceEnt
      x-api-path-slug: harvestsourceident-get
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
  /harvest/source/{ident}/jobs/:
    get:
      summary: Get Harvest Source Ent Jobs
      description: List all jobs for a given source
      operationId: getHarvestSourceEntJobs
      x-api-path-slug: harvestsourceidentjobs-get
      parameters:
      - in: path
        name: ident
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
      - Jobs
  /harvest/source/{ident}/preview:
    get:
      summary: Get Harvest Source Ent Preview
      description: Preview a single harvest source given an ID or a slug
      operationId: getHarvestSourceEntPreview
      x-api-path-slug: harvestsourceidentpreview-get
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
      - Preview
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