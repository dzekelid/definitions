---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine Get a health question definition
  description: Get a health question definition by id
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /health_question_definition:
    get:
      summary: List health question definitions
      description: Get a list of all health question definitions
      operationId: fetchHealthQuestionDefinitions
      x-api-path-slug: health-question-definition-get
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Health
      - Question
      - Definitions
  /health_question_definition/{id}:
    get:
      summary: Get a health question definition
      description: Get a health question definition by id
      operationId: fetchHealthQuestionDefinition
      x-api-path-slug: health-question-definitionid-get
      parameters:
      - in: path
        name: id
        description: Health question definition identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Health
      - Question
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