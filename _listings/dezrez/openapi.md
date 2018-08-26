---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/stats/visited/{entityType}:
    get:
      summary: Get all recent history of 'pages' visited on Rezi for a given entity
        type.
      description: Get all recent history of 'pages' visited on rezi for a given entity
        type..
      operationId: Stats_VisitedByentityType
      x-api-path-slug: apistatsvisitedentitytype-get
      parameters:
      - in: path
        name: entityType
        description: Either Groups, Properties or will default to all if nothing passed
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Recent
      - History
      - Of
      - Pages
      - Visited
      - "On"
      - Rezia
      - Given
      - Entity
      - Type
---