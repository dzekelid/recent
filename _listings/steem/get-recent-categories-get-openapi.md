---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get recent categories
  description: get tags
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_recent_categories:
    get:
      summary: get recent categories
      description: get tags
      operationId: get-tags
      x-api-path-slug: get-recent-categories-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Get
      - Recent
      - Categories
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