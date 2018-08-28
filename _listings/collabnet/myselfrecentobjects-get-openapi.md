---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Gets recent object list for the current
    user
  version: 1.0.0
  description: Gets recent object list for the current user.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /myself/recent/projects:
    get:
      summary: Gets recent project list for the current user
      description: Gets recent project list for the current user.
      operationId: getMyRecentProjects
      x-api-path-slug: myselfrecentprojects-get
      parameters:
      - in: query
        name: count
        description: Max
      responses:
        2:
          description: Successful response
        200:
          description: OK
      tags:
      - Recent
      - Project
      - Listthe
      - Current
      - User
  /myself/recent/objects:
    get:
      summary: Gets recent object list for the current user
      description: Gets recent object list for the current user.
      operationId: getMyRecentObjects
      x-api-path-slug: myselfrecentobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      responses:
        200:
          description: OK
      tags:
      - Recent
      - Object
      - Listthe
      - Current
      - User
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