---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 0
info:
  title: AP Metadata Services Ontology Definition
  description: Returns the AP ontology definition for the specified AP property or
    class and the specified format.
  version: v1
host: cv.ap.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  c/{class}.{format}:
    get:
      summary: Ontology Definition
      description: Returns the AP ontology definition for the specified AP property
        or class and the specified format.
      operationId: getCClass.Format
      x-api-path-slug: cclass-format-get
      parameters:
      - in: query
        name: apikey
        description: API Key
      - in: path
        name: class
        description: The name of an AP property or class
      - in: path
        name: format
        description: The format of the returned AP ontology data
      responses:
        200:
          description: OK
      tags:
      - Ontology
      - Definition
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