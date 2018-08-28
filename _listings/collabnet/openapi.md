swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
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