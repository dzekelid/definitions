---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 1
info:
  title: AP Metadata Services
  description: add-value-to-your-news-content-with-apu2019s-industryleading-metadata--accurate-comprehensive-richly-detailed-data-designed-specifically-for-use-by-news-publishers--ap-metadata-services-is-a-new-set-of-apis-that-gives-you-direct-access-to-the-same-metadata-system-that-supports-apu2019s-awardwinning-global-news-operation-
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
---