---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Gets the report definition template
  description: Return the report definition data object template
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
    post:
      summary: Create a new transform definition
      description: Creates a new transform defintion object
      operationId: PostTransformDefinition
      x-api-path-slug: transforms-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: TransformDefinition
        description: The transform definition object to be executed against the report
          data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Transform
      - Definition
  /Report/{ReportDefinitionId}:
    delete:
      summary: Deletes a report definition
      description: Delete the specified report definition
      operationId: DeleteReportDefinition
      x-api-path-slug: reportreportdefinitionid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
    get:
      summary: Get the report definition
      description: Returns the specified report definition from the authroised application
      operationId: GetReportDefinitionFromApplication
      x-api-path-slug: reportreportdefinitionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
    put:
      summary: Updates a report definition
      description: Updates the existing specified report definition object
      operationId: PutReportDefinition
      x-api-path-slug: reportreportdefinitionid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: ReportDefinition
        description: The report definition object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
  /Report/{ReportDefinitionId}/run:
    get:
      summary: Runs the specified report definition
      description: Returns the result of the executed report definition
      operationId: GetReportOutput
      x-api-path-slug: reportreportdefinitionidrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Specified
      - Report
      - Definition
  /Reports:
    post:
      summary: Create a new report definition
      description: Creates a new report defintion object
      operationId: PostReportDefinition
      x-api-path-slug: reports-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: ReportDefinition
        description: The report definition object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Report
      - Definition
  /Templates/reportdefinition:
    get:
      summary: Gets the report definition template
      description: Return the report definition data object template
      operationId: GetReportDefinitionTemplate
      x-api-path-slug: templatesreportdefinition-get
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
      - Report
      - Definition
      - Template
  /Transform/{TransformDefinitionId}:
    delete:
      summary: Deletes a transform definition
      description: Delete the specified transform definition
      operationId: DeleteTransformDefinition
      x-api-path-slug: transformtransformdefinitionid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: TransformDefinitionId
        description: The transform definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Transform
      - Definition
    get:
      summary: Get the transform definition
      description: Returns the specified transform definition from the authroised
        application
      operationId: GetTransformDefinitionFromApplication
      x-api-path-slug: transformtransformdefinitionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: TransformDefinitionId
        description: The transform definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Transform
      - Definition
    put:
      summary: Updates a transform definition
      description: Updates the existing specified transform definition object
      operationId: PutTransformDefinition
      x-api-path-slug: transformtransformdefinitionid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: TransformDefinition
        description: The transform definition object to be executed against the report
          data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: TransformDefinitionId
        description: The transform definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Transform
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