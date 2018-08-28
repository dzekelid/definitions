swagger: "2.0"
x-collection-name: Brookline Massachusetts 311
x-complete: 1
info:
  title: Brookline MA Open311 GeoReport API
  description: open311-allows-you-to-getpost-civic-information-of-cities-via-a-unified-interface--the-georeport-part-allows-you-to-submit-and-view-issues-at-the-public-local-space
  termsOfService: (depends on server instance for example NYC http://dev.cityofchicago.org/docs/api/tos)
  contact:
    name: Open311 community
    url: http://wiki.open311.org/GeoReport_v2/
    email: discuss@lists.open311.org
  version: 1.0.0
host: spot.brooklinema.gov
basePath: /open311/v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /services/{service_code}.{response_format}:
    get:
      summary: (extended) Definition Of A Service Type
      description: Define attributes associated with a service code. These attributes
        can be unique to the city/jurisdiction.
      operationId: define-attributes-associated-with-a-service-code-these-attributes-can-be-unique-to-the-cityjurisdict
      x-api-path-slug: servicesservice-code-response-format-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: service_code
      responses:
        200:
          description: OK
      tags:
      - "311"
      - (extended)
      - Definition
      - Service
      - Type