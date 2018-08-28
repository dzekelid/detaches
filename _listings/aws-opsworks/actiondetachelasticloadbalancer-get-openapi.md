---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 0
info:
  title: AWS OpsWorks API Detach Elastic Load Balancer
  version: 1.0.0
  description: Detaches a specified Elastic Load Balancing instance from its layer.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DetachElasticLoadBalancer:
    get:
      summary: Detach Elastic Load Balancer
      description: Detaches a specified Elastic Load Balancing instance from its layer.
      operationId: detachElasticLoadBalancer
      x-api-path-slug: actiondetachelasticloadbalancer-get
      parameters:
      - in: query
        name: ElasticLoadBalancerName
        description: The Elastic Load Balancing instances name
        type: string
      - in: query
        name: LayerId
        description: The ID of the layer that the Elastic Load Balancing instance
          is attached to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Detach
      - Elastic
      - Load
      - Balancer
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