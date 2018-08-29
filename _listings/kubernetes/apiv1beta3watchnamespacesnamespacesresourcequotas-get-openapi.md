---
swagger: "2.0"
x-collection-name: Kubernetes
x-complete: 0
info:
  title: Kubernetes Get Watch Namespaces Resourcequotas
  version: 1.0.0
  description: Watch a list of resourcequota.
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
  /api/v1beta3/watch/namespaces/{namespaces}/limitranges:
    get:
      summary: Get Watch Namespaces Limitranges
      description: Watch a list of limitrange.
      operationId: watchLimitRangelist
      x-api-path-slug: apiv1beta3watchnamespacesnamespaceslimitranges-get
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
      - Limitranges
  /api/v1beta3/watch/namespaces/{namespaces}/limitranges/{name}:
    get:
      summary: Get Watch Namespaces Limitranges Name
      description: Watch a particular limitrange.
      operationId: watchLimitRange
      x-api-path-slug: apiv1beta3watchnamespacesnamespaceslimitrangesname-get
      parameters:
      - in: path
        name: name
        description: name of the LimitRange
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Limitranges
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/pods:
    get:
      summary: Get Watch Namespaces Pods
      description: Watch a list of pod.
      operationId: watchPodlist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacespods-get
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
      - Pods
  /api/v1beta3/watch/namespaces/{namespaces}/pods/{name}:
    get:
      summary: Get Watch Namespaces Pods Name
      description: Watch a particular pod.
      operationId: watchPod
      x-api-path-slug: apiv1beta3watchnamespacesnamespacespodsname-get
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Pods
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/replicationcontrollers:
    get:
      summary: Get Watch Namespaces Replicationcontrollers
      description: Watch a list of replicationcontroller.
      operationId: watchReplicationControllerlist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesreplicationcontrollers-get
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
      - Replicationcontrollers
  /api/v1beta3/watch/namespaces/{namespaces}/replicationcontrollers/{name}:
    get:
      summary: Get Watch Namespaces Replicationcontrollers Name
      description: Watch a particular replicationcontroller.
      operationId: watchReplicationController
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesreplicationcontrollersname-get
      parameters:
      - in: path
        name: name
        description: name of the ReplicationController
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Replicationcontrollers
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/resourcequotas:
    get:
      summary: Get Watch Namespaces Resourcequotas
      description: Watch a list of resourcequota.
      operationId: watchResourceQuotalist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesresourcequotas-get
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
      - Resourcequotas
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