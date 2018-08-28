---
swagger: "2.0"
x-collection-name: AWS Data Pipeline
x-complete: 0
info:
  title: AWS Data Pipeline API Get Pipeline Definition
  version: 1.0.0
  description: Gets the definition of the specified pipeline.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetPipelineDefinition:
    get:
      summary: Get Pipeline Definition
      description: Gets the definition of the specified pipeline.
      operationId: getPipelineDefinition
      x-api-path-slug: actiongetpipelinedefinition-get
      parameters:
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: version
        description: The version of the pipeline definition to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
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