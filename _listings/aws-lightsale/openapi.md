---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DetachStaticIp:
    get:
      summary: Detach Static Ip
      description: |-
        Detaches a static IP from the Amazon Lightsail instance to which it is
              attached.
      operationId: detachStaticIp
      x-api-path-slug: actiondetachstaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP to detach from the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
---