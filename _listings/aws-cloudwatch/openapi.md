swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 1
info:
  title: AWS CloudWatch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutMetricData:
    "":
      summary: Put Metric Data
      description: Publishes metric data points to Amazon CloudWatch.
      operationId: putmetricdata
      x-api-path-slug: actionputmetricdata-
      parameters:
      - in: query
        name: MetricData.member.N
        description: The data for the metric
        type: string
      - in: query
        name: Namespace
        description: The namespace for the metric data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Data Metric