---
swagger: "2.0"
x-collection-name: Wordnik
x-complete: 1
info:
  title: Wordnik
  description: wordnik-is-the-worlds-biggest-online-english-dictionary-by-number-of-words
  version: "4.0"
host: api.wordnik.com
basePath: /v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /word.json/{word}/definitions:
    get:
      summary: Return definitions for a word
      description: Return definitions for a word.
      operationId: getDefinitions
      x-api-path-slug: word-jsonworddefinitions-get
      parameters:
      - in: query
        name: includeRelated
        description: Return related words with definitions
      - in: query
        name: includeTags
        description: Return a closed set of XML tags in response
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: partOfSpeech
        description: CSV list of part-of-speech types
      - in: query
        name: sourceDictionaries
        description: Source dictionary to return definitions from
      - in: query
        name: useCanonical
        description: If true will try to return the correct word root (cats -> cat)
      - in: path
        name: word
        description: Word to return definitions for
      responses:
        200:
          description: OK
      tags:
      - Words
      - Definitions
---