---
swagger: "2.0"
x-collection-name: Backupify
x-complete: 0
info:
  title: Backupify Create a new variable for the specified key for the specified backup_definition
  description: It is only possible to create variables for backup_definitions you
    have permission to manage.
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
    post:
      summary: Create a new backup_definition
      description: Create a new backup_definition.
      operationId: postV1BackupDefinitions
      x-api-path-slug: v1backup-definitions-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: backup_definition[description]
        description: Description of the backup_definition
      - in: formData
        name: backup_definition[name]
        description: Name for the backup_definition
      - in: formData
        name: backup_definition[published]
        description: Boolean flag indicating whether the backup definition is published
          and available for use
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
  /v1/backup_definitions/{backup_definition_id}:
    get:
      summary: Retrieve a backup_definition by backup_definition_id
      description: Only backup_definitions you have permission to view will be returned
      operationId: getV1BackupDefinitionsBackupDefinition
      x-api-path-slug: v1backup-definitionsbackup-definition-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
    put:
      summary: Update the specified backup_definition
      description: Only backup_definitions you have permission to change can be modified
      operationId: putV1BackupDefinitionsBackupDefinition
      x-api-path-slug: v1backup-definitionsbackup-definition-id-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: backup_definition[description]
        description: Description of the backup_definition
      - in: formData
        name: backup_definition[name]
        description: Name for the backup_definition
      - in: formData
        name: backup_definition[published]
        description: Boolean flag indicating whether the backup definition is published
          and available for use
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
  /v1/backup_definitions/{backup_definition_id}/variables:
    get:
      summary: Retrieve a list of variables for the specified backup_definition
      description: You can only retrieve variables for backup_definitions you have
        access to. Records are returned in ascending order (by id), with a default
        of 20 per page. Links to the next, previous, first, and last pages can be
        found in the response headers.
      operationId: getV1BackupDefinitionsBackupDefinitionVariables
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariables-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve variables for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
    post:
      summary: Create a new variable for the specified key for the specified backup_definition
      description: It is only possible to create variables for backup_definitions
        you have permission to manage.
      operationId: postV1BackupDefinitionsBackupDefinitionVariables
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariables-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to create a variable for
      - in: formData
        name: variable[default_value]
        description: A default value that can be used when no instance specific value
          is provided
      - in: formData
        name: variable[description]
        description: Description offering additional information or detail about the
          variable
      - in: formData
        name: variable[key]
        description: The symbolic name or identifier to access the defined variable
          by
      - in: formData
        name: variable[name]
        description: A human-friendly name for the variable
      - in: formData
        name: variable[optional]
        description: Flag indicating whether this variable is optional or if a value
          is required
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
  /v1/backup_definitions/{backup_definition_id}/variables/{key}:
    get:
      summary: Retrieve a specific variable by key for the specified backup_definition
      description: You can only retrieve variables for backup_definitions you have
        access to
      operationId: getV1BackupDefinitionsBackupDefinitionVariablesKey
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariableskey-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve a variable for
      - in: path
        name: key
        description: The key, symbolic name, or identifier of the variable to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
      - Key
    put:
      summary: Update a specific variable by key for the specified backup_definition
      description: You can only update variables for backup_definitions you have access
        to. Additionally, it is not possible to update a variable's key. Requests
        including a modified key name will result in an error.
      operationId: putV1BackupDefinitionsBackupDefinitionVariablesKey
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariableskey-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve a variable for
      - in: path
        name: key
        description: The key, symbolic name, or identifier of the variable to update
      - in: formData
        name: name
        description: The human-friendly name to use for the variable
      - in: formData
        name: variable[default_value]
        description: A default value that can be used when no instance specific value
          is provided
      - in: formData
        name: variable[description]
        description: Description offering additional information or detail about the
          variable
      - in: formData
        name: variable[optional]
        description: Flag indicating whether this variable is optional or if a value
          is required
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
      - Key
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