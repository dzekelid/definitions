---
swagger: "2.0"
x-collection-name: AWS Data Pipeline
x-complete: 1
info:
  title: AWS Data Pipeline API
  version: 1.0.0
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
  /?Action=PutPipelineDefinition:
    get:
      summary: Put Pipeline Definition
      description: Adds tasks, schedules, and preconditions to the specified pipeline.
      operationId: putPipelineDefinition
      x-api-path-slug: actionputpipelinedefinition-get
      parameters:
      - in: query
        name: parameterObjects
        description: The parameter objects used with the pipeline
        type: string
      - in: query
        name: parameterValues
        description: The parameter values used with the pipeline
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: pipelineObjects
        description: The objects that define the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=ValidatePipelineDefinition:
    get:
      summary: Validate Pipeline Definition
      description: Validates the specified pipeline definition to ensure that it is
        well formed and can be run without error.
      operationId: validatePipelineDefinition
      x-api-path-slug: actionvalidatepipelinedefinition-get
      parameters:
      - in: query
        name: parameterObjects
        description: The parameter objects used with the pipeline
        type: string
      - in: query
        name: parameterValues
        description: The parameter values used with the pipeline
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: pipelineObjects
        description: The objects that define the pipeline changes to validate against
          the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
---