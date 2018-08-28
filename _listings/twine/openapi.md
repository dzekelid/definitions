swagger: "2.0"
x-collection-name: Twine
x-complete: 1
info:
  title: Twine
  description: -overviewthe-twine-health-api-is-restful-api--the-requests-and-responses-are-formated-according-to-the-json-apihttpjsonapi-orgformat1-0-specification-in-addition-to-this-documentation-we-also-provide-an-openapihttpsgithub-comoaiopenapispecificationblobmasterversions2-0-md-yaml-file-describing-the-api-twine-api-specificationswagger-yaml--authenticationauthentication-for-the-twine-api-is-based-on-the-oauth-2-0-authorization-frameworkhttpstools-ietf-orghtmlrfc6749--twine-currently-supports-grant-types-of-client-credentials-and-refresh-token-see-post-oauthtokenoperationcreatetoken-for-details-on-the-request-and-response-formats--redocinject-securitydefinitions-
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