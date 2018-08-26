---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
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
---