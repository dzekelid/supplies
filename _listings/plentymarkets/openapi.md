swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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