---
name: APIs.Guru
x-slug: apis-guru
description: 'Our goal is to create a machine-readable Wikipedia for REST APIs with
  the following principal: Open source, community driven project. Only publicly available
  APIs (free or paid). Anyone can add or change an API, not only API owners. All data
  can be accessed through a REST API'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2018-05-21 at 3.08.45 PM.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Definitions
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/apis-guru/apis.md
specificationVersion: "0.14"
apis:
- name: APIs.guru - List all APIs
  x-api-slug: list-json-get
  description: |-
    List all APIs in the directory.
    Returns links to OpenAPI specification for each API in the directory.
    If API exist in multiple versions `preferred` one is explicitly marked.

    Some basic info from OpenAPI spec is cached inside each object.
    This allows to generate some simple views without need to fetch OpenAPI spec for each API.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-05-21 at 3.08.45 PM.png
  humanURL: http://apis.guru
  baseURL: https://api.apis.guru//v2/
  tags: Discovery, API Service Provider, API Tool, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/apis-guru/list-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/apis-guru/list-json-get-openapi.md
- name: APIs.guru - Get basic metrics
  x-api-slug: metrics-json-get
  description: |-
    Some basic metrics for the entire directory.
    Just stunning numbers to put on a front page and are intended purely for WoW effect :)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-05-21 at 3.08.45 PM.png
  humanURL: http://apis.guru
  baseURL: https://api.apis.guru//v2/
  tags: Discovery, API Service Provider, API Tool, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/apis-guru/metrics-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/apis-guru/metrics-json-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://apimetrics.api.gallery.streamdata.io
- type: x-api-stack
  url: http://apis.guru.stack.network
- type: x-website
  url: http://apis.guru
- type: x-website
  url: https://apis.guru/openapi-directory/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---