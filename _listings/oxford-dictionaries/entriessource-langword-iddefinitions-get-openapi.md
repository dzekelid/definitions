---
swagger: "2.0"
x-collection-name: Oxford Dictionaries
x-complete: 0
info:
  title: Oxford Dictionaries Retrieve only definitions in entry search.
  description: Find available [dictionary entries](/glossary?tag=#entry&expand) for
    given word and language. Filter results by categories.
  termsOfService: http://helloreverb.com/terms/
  version: 1.8.0
host: od-api-demo.oxforddictionaries.com:443
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /entries/{source_lang}/{word_id}/definitions:
    get:
      summary: Retrieve only definitions in entry search.
      description: Find available [dictionary entries](/glossary?tag=#entry&expand)
        for given word and language. Filter results by categories.
      operationId: getEntriesSourceLangWordDefinitions
      x-api-path-slug: entriessource-langword-iddefinitions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Entries
      - Source
      - Lang
      - Word
      - Id
      - Definitions
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