---
swagger: "2.0"
x-collection-name: Kubernetes
x-complete: 0
info:
  title: Kubernetes Get Watch Namespaces Events Name
  version: 1.0.0
  description: Watch a particular event.
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
  /api/v1beta3/watch/limitranges:
    get:
      summary: Get Watch Limitranges
      description: Watch a list of limitrange.
      operationId: watchLimitRangelist
      x-api-path-slug: apiv1beta3watchlimitranges-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Limitranges
  /api/v1beta3/watch/namespaces:
    get:
      summary: Get Watch Namespaces
      description: Watch a list of namespace.
      operationId: watchNamespacelist
      x-api-path-slug: apiv1beta3watchnamespaces-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
  /api/v1beta3/watch/namespaces/{namespaces}/endpoints:
    get:
      summary: Get Watch Namespaces Endpoints
      description: Watch a list of endpoints.
      operationId: watchEndpointslist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesendpoints-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Endpoints
  /api/v1beta3/watch/namespaces/{namespaces}/endpoints/{name}:
    get:
      summary: Get Watch Namespaces Endpoints Name
      description: Watch a particular endpoints.
      operationId: watchEndpoints
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesendpointsname-get
      parameters:
      - in: path
        name: name
        description: name of the Endpoints
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Endpoints
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/events:
    get:
      summary: Get Watch Namespaces Events
      description: Watch a list of event.
      operationId: watchEventlist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesevents-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Events
  /api/v1beta3/watch/namespaces/{namespaces}/events/{name}:
    get:
      summary: Get Watch Namespaces Events Name
      description: Watch a particular event.
      operationId: watchEvent
      x-api-path-slug: apiv1beta3watchnamespacesnamespaceseventsname-get
      parameters:
      - in: path
        name: name
        description: name of the Event
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Events
      - Name
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