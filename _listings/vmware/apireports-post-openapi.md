---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Generate a report
  description: |-
    You will need to update several items in the body such as:
      - ID of resource you wish to run this report on
      - ID of the report you wish to run
      - Traversal Spec for the report (you can get this from the API query
    "Get Report Definitions", the travesal spec must match the resource type.
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/reportdefinitions:
    get:
      summary: Get Report Definitions
      description: Gets all - to get a single report ID, just add /<report def id>
      operationId: ApiReportdefinitionsGet
      x-api-path-slug: apireportdefinitions-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Reportdefinitions
  /api/reports:
    post:
      summary: Generate a report
      description: |-
        You will need to update several items in the body such as:
          - ID of resource you wish to run this report on
          - ID of the report you wish to run
          - Traversal Spec for the report (you can get this from the API query
        "Get Report Definitions", the travesal spec must match the resource type.
      operationId: ApiReportsPost
      x-api-path-slug: apireports-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Reports
  /api/alertdefinitions/{alertDefinitionId}:
    get:
      summary: Get Alert Definition
      description: 'TODO: Add Description'
      operationId: ApiAlertdefinitionsByAlertDefinitionIdGet
      x-api-path-slug: apialertdefinitionsalertdefinitionid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: alertDefinitionId
      responses:
        200:
          description: OK
      tags:
      - Alertdefinitions
      - AlertDefinitionId
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