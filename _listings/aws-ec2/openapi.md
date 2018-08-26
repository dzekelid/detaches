---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DetachInternetGateway:
    get:
      summary: Detach Internet Gateway
      description: Detaches an Internet gateway from a VPC, disabling connectivity
        between the Internet and the VPC.
      operationId: detachinternetgateway
      x-api-path-slug: actiondetachinternetgateway-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: KeyName
        description: A unique name for the key pair
        type: string
      responses:
        200:
          description: OK
      tags:
      - Internet Gateway
  /?Action=DetachNetworkInterface:
    get:
      summary: Detach Network Interface
      description: Detaches a network interface from an instance.
      operationId: detachnetworkinterface
      x-api-path-slug: actiondetachnetworkinterface-get
      parameters:
      - in: query
        name: Attachment
        description: Information about the interface attachment
        type: string
      - in: query
        name: Description
        description: A description for the network interface
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: SecurityGroupId.N
        description: Changes the security groups for the network interface
        type: string
      - in: query
        name: SourceDestCheck
        description: Indicates whether source/destination checking is enabled
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network Interface
  /?Action=DetachVolume:
    get:
      summary: Detach Volume
      description: Detaches an EBS volume from an instance.
      operationId: detachvolume
      x-api-path-slug: actiondetachvolume-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volume
---