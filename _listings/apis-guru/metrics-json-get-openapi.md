---
swagger: "2.0"
x-collection-name: APIs.Guru
x-complete: 0
info:
  title: APIs.guru Get basic metrics
  description: |-
    Some basic metrics for the entire directory.
    Just stunning numbers to put on a front page and are intended purely for WoW effect :)
  contact:
    name: APIs.guru
    url: http://APIs.guru
    email: founders@apis.guru
  version: 2.0.1
host: api.apis.guru
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /list.json:
    get:
      summary: List all APIs
      description: |-
        List all APIs in the directory.
        Returns links to OpenAPI specification for each API in the directory.
        If API exist in multiple versions `preferred` one is explicitly marked.

        Some basic info from OpenAPI spec is cached inside each object.
        This allows to generate some simple views without need to fetch OpenAPI spec for each API.
      operationId: listAPIs
      x-api-path-slug: list-json-get
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Definitions
      - Discovery
  /metrics.json:
    get:
      summary: Get basic metrics
      description: |-
        Some basic metrics for the entire directory.
        Just stunning numbers to put on a front page and are intended purely for WoW effect :)
      operationId: getMetrics
      x-api-path-slug: metrics-json-get
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Definitions
      - Discovery
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