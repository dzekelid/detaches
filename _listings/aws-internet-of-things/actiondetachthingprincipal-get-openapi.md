---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 0
info:
  title: AWS Internet of Things API Detach Thing Principal
  version: 1.0.0
  description: Detaches the specified principal from the specified thing.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DetachThingPrincipal:
    get:
      summary: Detach Thing Principal
      description: Detaches the specified principal from the specified thing.
      operationId: detachThingPrincipal
      x-api-path-slug: actiondetachthingprincipal-get
      parameters:
      - in: query
        name: principal
        description: If the principal is a certificate, this value must be ARN of
          the certificate
        type: string
      - in: query
        name: thingName
        description: The name of the thing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Principals
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