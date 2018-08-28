---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 0
info:
  title: Amazon EC2 Container Service API Deregister Task Definition
  version: 1.0.0
  description: Deregisters the specified task definition by family and revision.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListTaskDefinitions:
    get:
      summary: List Task Definitions
      description: Returns a list of task definitions that are registered to your
        account.
      operationId: listTaskDefinitions
      x-api-path-slug: actionlisttaskdefinitions-get
      parameters:
      - in: query
        name: familyPrefix
        description: The full family name with which to filter the ListTaskDefinitions            results
        type: string
      - in: query
        name: maxResults
        description: The maximum number of task definition results returned by                ListTaskDefinitions
          in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListTaskDefinitions
          request where maxResults was used and            the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: sort
        description: The order in which to sort the results
        type: string
      - in: query
        name: status
        description: The task definition status with which to filter the                ListTaskDefinitions
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=RegisterTaskDefinition:
    get:
      summary: Register Task Definition
      description: |-
        Registers a new task definition from the supplied family and
                        containerDefinitions.
      operationId: registerTaskDefinition
      x-api-path-slug: actionregistertaskdefinition-get
      parameters:
      - in: query
        name: containerDefinitions
        description: A list of container definitions in JSON format that describe
          the different            containers that make up your task
        type: string
      - in: query
        name: family
        description: You must specify a family for a task definition, which allows
          you to            track multiple versions of the same task definition
        type: string
      - in: query
        name: networkMode
        description: The Docker networking mode to use for the containers in the task
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for the task
        type: string
      - in: query
        name: taskRoleArn
        description: The short name or full Amazon Resource Name (ARN) of the IAM
          role that containers in this task can            assume
        type: string
      - in: query
        name: volumes
        description: A list of volume definitions in JSON format that containers in
          your task may            use
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=DeregisterTaskDefinition:
    get:
      summary: Deregister Task Definition
      description: Deregisters the specified task definition by family and revision.
      operationId: deregisterTaskDefinition
      x-api-path-slug: actionderegistertaskdefinition-get
      parameters:
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to deregister
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
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