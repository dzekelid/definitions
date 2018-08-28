---
name: Backupify
x-slug: backupify
description: ""
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Definitions
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/apis.md
specificationVersion: "0.14"
apis:
- name: Backupify - Retrieve an index of all backup_definitions
  x-api-slug: v1backup-definitions-get
  description: This will retrieve a list of backup_defintions from all vendors. To
    view backup_defintions for a particular vendor, see the vendors API. Records are
    returned in ascending order (by id), with a default of 20 per page. Links to the
    next, previous, first, and last pages can be found in the response headers.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitions-get-openapi.md
- name: Backupify - Create a new backup_definition
  x-api-slug: v1backup-definitions-post
  description: Create a new backup_definition.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitions-post-openapi.md
- name: Backupify - Retrieve a backup_definition by backup_definition_id
  x-api-slug: v1backup-definitionsbackup-definition-id-get
  description: Only backup_definitions you have permission to view will be returned
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-get-openapi.md
- name: Backupify - Update the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-id-put
  description: Only backup_definitions you have permission to change can be modified
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-put-openapi.md
- name: Backupify - Retrieve a list of variables for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariables-get
  description: You can only retrieve variables for backup_definitions you have access
    to. Records are returned in ascending order (by id), with a default of 20 per
    page. Links to the next, previous, first, and last pages can be found in the response
    headers.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-get-openapi.md
- name: Backupify - Create a new variable for the specified key for the specified
    backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariables-post
  description: It is only possible to create variables for backup_definitions you
    have permission to manage.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-post-openapi.md
- name: Backupify - Retrieve a specific variable by key for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariableskey-get
  description: You can only retrieve variables for backup_definitions you have access
    to
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-get-openapi.md
- name: Backupify - Update a specific variable by key for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariableskey-put
  description: You can only update variables for backup_definitions you have access
    to. Additionally, it is not possible to update a variable's key. Requests including
    a modified key name will result in an error.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-put-openapi.md
- name: Backupify - Retrieve a backup_definition by backup_definition_id
  x-api-slug: v1backup-definitionsbackup-definition-id-get
  description: Only backup_definitions you have permission to view will be returned
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-get-openapi.md
- name: Backupify - Update the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-id-put
  description: Only backup_definitions you have permission to change can be modified
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-put-openapi.md
- name: Backupify - Retrieve a list of variables for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariables-get
  description: You can only retrieve variables for backup_definitions you have access
    to. Records are returned in ascending order (by id), with a default of 20 per
    page. Links to the next, previous, first, and last pages can be found in the response
    headers.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-get-openapi.md
- name: Backupify - Create a new variable for the specified key for the specified
    backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariables-post
  description: It is only possible to create variables for backup_definitions you
    have permission to manage.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-post-openapi.md
- name: Backupify - Retrieve a specific variable by key for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariableskey-get
  description: You can only retrieve variables for backup_definitions you have access
    to
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-get-openapi.md
- name: Backupify - Update a specific variable by key for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariableskey-put
  description: You can only update variables for backup_definitions you have access
    to. Additionally, it is not possible to update a variable's key. Requests including
    a modified key name will result in an error.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-put-openapi.md
- name: Backupify - Retrieve a backup_definition by backup_definition_id
  x-api-slug: v1backup-definitionsbackup-definition-id-get
  description: Only backup_definitions you have permission to view will be returned
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-get-openapi.md
- name: Backupify - Update the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-id-put
  description: Only backup_definitions you have permission to change can be modified
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-put-openapi.md
- name: Backupify - Retrieve a list of variables for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariables-get
  description: You can only retrieve variables for backup_definitions you have access
    to. Records are returned in ascending order (by id), with a default of 20 per
    page. Links to the next, previous, first, and last pages can be found in the response
    headers.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-get-openapi.md
- name: Backupify - Create a new variable for the specified key for the specified
    backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariables-post
  description: It is only possible to create variables for backup_definitions you
    have permission to manage.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-post-openapi.md
- name: Backupify - Retrieve a specific variable by key for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariableskey-get
  description: You can only retrieve variables for backup_definitions you have access
    to
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-get-openapi.md
- name: Backupify - Update a specific variable by key for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariableskey-put
  description: You can only update variables for backup_definitions you have access
    to. Additionally, it is not possible to update a variable's key. Requests including
    a modified key name will result in an error.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-put-openapi.md
- name: Backupify - Update a specific variable by key for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariableskey-put
  description: You can only update variables for backup_definitions you have access
    to. Additionally, it is not possible to update a variable's key. Requests including
    a modified key name will result in an error.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-put-openapi.md
- name: Backupify - Retrieve a specific variable by key for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariableskey-get
  description: You can only retrieve variables for backup_definitions you have access
    to
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariableskey-get-openapi.md
- name: Backupify - Create a new variable for the specified key for the specified
    backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariables-post
  description: It is only possible to create variables for backup_definitions you
    have permission to manage.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-post-openapi.md
- name: Backupify - Retrieve a list of variables for the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-idvariables-get
  description: You can only retrieve variables for backup_definitions you have access
    to. Records are returned in ascending order (by id), with a default of 20 per
    page. Links to the next, previous, first, and last pages can be found in the response
    headers.
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-idvariables-get-openapi.md
- name: Backupify - Update the specified backup_definition
  x-api-slug: v1backup-definitionsbackup-definition-id-put
  description: Only backup_definitions you have permission to change can be modified
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-put-openapi.md
- name: Backupify - Retrieve a backup_definition by backup_definition_id
  x-api-slug: v1backup-definitionsbackup-definition-id-get
  description: Only backup_definitions you have permission to view will be returned
  image: ""
  humanURL: http://backupify.com
  baseURL: https://api.backupify.com//
  tags: API Not Found, API Provider, Backups, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/definitions/master/_listings/backupify/v1backup-definitionsbackup-definition-id-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.virtual.network.api.gallery.streamdata.io
- type: x-api-stack
  url: http://backupify.stack.network
- type: x-blog
  url: https://www.backupify.com/blog
- type: x-website
  url: http://backupify.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---