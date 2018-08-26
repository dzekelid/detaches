---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DetachLoadBalancers:
    get:
      summary: Detach Load Balancers
      description: Detaches one or more Classic load balancers from the specified
        Auto Scaling group.
      operationId: detachLoadBalancers
      x-api-path-slug: actiondetachloadbalancers-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: LoadBalancerNames.member.N
        description: One or more load balancer names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DetachLoadBalancerTargetGroups:
    get:
      summary: Detach Load Balancer Target Groups
      description: Detaches one or more target groups from the specified Auto Scaling
        group.
      operationId: detachLoadBalancerTargetGroups
      x-api-path-slug: actiondetachloadbalancertargetgroups-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: TargetGroupARNs.member.N
        description: The Amazon Resource Names (ARN) of the target groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
---