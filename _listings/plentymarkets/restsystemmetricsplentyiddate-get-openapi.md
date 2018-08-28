---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Supply usage data for given plentymarkets system
  description: Supply usage data for given plentymarkets system.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/system/metrics/{plentyId}/{date}:
    get:
      summary: Supply usage data for given plentymarkets system
      description: Supply usage data for given plentymarkets system.
      operationId: getRestSystemMetricsPlentyDate
      x-api-path-slug: restsystemmetricsplentyiddate-get
      parameters:
      - in: path
        name: date
      - in: path
        name: plentyId
      responses:
        200:
          description: OK
      tags:
      - Supply
      - Usage
      - Datagiven
      - Plentymarkets
      - System
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