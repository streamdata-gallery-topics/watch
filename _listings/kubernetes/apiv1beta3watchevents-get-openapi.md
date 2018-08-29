---
swagger: "2.0"
x-collection-name: Kubernetes
x-complete: 0
info:
  title: Kubernetes Get Watch Events
  version: 1.0.0
  description: Watch a list of event.
host: /api/v1beta3
basePath: 127.0.0.1:6443
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1beta3/watch/endpoints:
    get:
      summary: Get Watch Endpoints
      description: Watch a list of endpoints.
      operationId: watchEndpointslist
      x-api-path-slug: apiv1beta3watchendpoints-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Endpoints
  /api/v1beta3/watch/events:
    get:
      summary: Get Watch Events
      description: Watch a list of event.
      operationId: watchEventlist
      x-api-path-slug: apiv1beta3watchevents-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Events
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