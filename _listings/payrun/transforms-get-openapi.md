---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Gets all transform definitions
  description: Get links to all saved transform definitions under authorised application
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Transforms:
    get:
      summary: Gets all transform definitions
      description: Get links to all saved transform definitions under authorised application
      operationId: GetTransformDefinitionsFromApplication
      x-api-path-slug: transforms-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ""
      - Transform
      - Definitions
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