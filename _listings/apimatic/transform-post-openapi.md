---
swagger: "2.0"
x-collection-name: APIMATIC
x-complete: 0
info:
  title: APIMATIC API Transformer Transform API Descriptions from/to various formats
  description: |-
    Transform API Descriptions from/to various formats e.g., Swagger, API Blueprint, RAML, WADL, Google Discovery, I/O Docs.

    ### INPUTS
    * API Blueprint
    * Swagger 1.0 - 1.2
    * Swagger 2.0 JSON
    * Swagger 2.0 YAML
    * WADL - W3C 2009
    * Google Discovery
    * RAML 0.8
    * I/O Docs - Mashery
    * HAR 1.2
    * Postman Collection 1.0 - 2.0
    * APIMATIC Format
    * Mashape

    ### OUTPUTS
    * API Blueprint
    * Swagger 1.2
    * Swagger 2.0 JSON
    * Swagger 2.0 YAML
    * WADL - W3C 2009
    * RAML 0.8 - 1.0
    * APIMATIC Format
  termsOfService: https://apimatic.io/transformer
  contact:
    name: API Transformer
    url: https://apimatic.io/transformer
    email: transform@apimatic.io
  version: "1.0"
host: apimatic.io
basePath: /api/transform
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transform:
    post:
      summary: Transform API Descriptions from/to various formats
      description: |-
        Transform API Descriptions from/to various formats e.g., Swagger, API Blueprint, RAML, WADL, Google Discovery, I/O Docs.

        ### INPUTS
        * API Blueprint
        * Swagger 1.0 - 1.2
        * Swagger 2.0 JSON
        * Swagger 2.0 YAML
        * WADL - W3C 2009
        * Google Discovery
        * RAML 0.8
        * I/O Docs - Mashery
        * HAR 1.2
        * Postman Collection 1.0 - 2.0
        * APIMATIC Format
        * Mashape

        ### OUTPUTS
        * API Blueprint
        * Swagger 1.2
        * Swagger 2.0 JSON
        * Swagger 2.0 YAML
        * WADL - W3C 2009
        * RAML 0.8 - 1.0
        * APIMATIC Format
      operationId: ConvertAPI
      x-api-path-slug: transform-post
      parameters:
      - in: query
        name: format
      - in: formData
        name: url
      responses:
        200:
          description: OK
      tags:
      - API Definition
      - Conversion
      - Tranform
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