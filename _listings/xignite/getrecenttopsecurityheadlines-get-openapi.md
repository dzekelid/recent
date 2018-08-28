---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global News Get Recent Top Security Headlines
  description: Returns 14 days specified number of headlines for a given security.
  version: 1.0.0
host: globalnews.xignite.com
basePath: xGlobalNews.xml/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetMostRecentEventsByEventCode:
    get:
      summary: Get Most Recent Events By Event Code
      description: Get the most recent events based on the event code and count.
      operationId: postGetmostrecenteventsbyeventcode
      x-api-path-slug: getmostrecenteventsbyeventcode-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Most
      - Recent
      - Events
      - Event
      - Code
  /GetRecentTopSecurityHeadlines:
    get:
      summary: Get Recent Top Security Headlines
      description: Returns 14 days specified number of headlines for a given security.
      operationId: GetRecentTopSecurityHeadlines
      x-api-path-slug: getrecenttopsecurityheadlines-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Recent
      - Top
      - Security
      - Headlines
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