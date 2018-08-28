swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/scheduler/jobs:
    get:
      summary: Get all job definition entries.
      description: Returns all job definition entries as specified by page and sort
        criteria.
      operationId: retrieveAllJobs
      x-api-path-slug: apiv1schedulerjobs-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: query
        name: page
        description: 'page index : zero-based page index'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: size
        description: 'page size : between 1 and 1000 inclusive'
      - in: query
        name: sortOrder
        description: 'sort order : asc | desc'
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Job
      - Definition
      - Entries
  /api/v1/scheduler/jobs/{id}:
    delete:
      summary: Delete job definition.
      description: Delete job definition for the given job id.
      operationId: deleteJob
      x-api-path-slug: apiv1schedulerjobsid-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Job id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Job
      - Definition