---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Checkins Recent
  description: /checkins/add
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /checkins/recent:
    get:
      summary: Get Checkins Recent
      description: /checkins/add
      operationId: checkinsadd
      x-api-path-slug: checkinsrecent-get
      parameters:
      - in: query
        name: afterTimestamp
        description: Seconds after which to look for checkins, e
      - in: query
        name: limit
        description: Number of results to return, up to 100
      - in: query
        name: ll
        description: Latitude and longitude of the users location, so response can
          include distance
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Checkins
      - Recent
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