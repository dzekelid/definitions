---
swagger: "2.0"
x-collection-name: Backupify
x-complete: 0
info:
  title: Backupify Retrieve an index of all backup_definitions
  description: This will retrieve a list of backup_defintions from all vendors. To
    view backup_defintions for a particular vendor, see the vendors API. Records are
    returned in ascending order (by id), with a default of 20 per page. Links to the
    next, previous, first, and last pages can be found in the response headers.
  version: 1.0.0
host: api.backupify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/backup_definitions:
    get:
      summary: Retrieve an index of all backup_definitions
      description: This will retrieve a list of backup_defintions from all vendors.
        To view backup_defintions for a particular vendor, see the vendors API. Records
        are returned in ascending order (by id), with a default of 20 per page. Links
        to the next, previous, first, and last pages can be found in the response
        headers.
      operationId: getV1BackupDefinitions
      x-api-path-slug: v1backup-definitions-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: query
        name: vendor_id
        description: Limit backup_definitions returned to those owned by the specified
          vendor_id
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
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