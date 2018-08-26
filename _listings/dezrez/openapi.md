---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branding/{id}/detachdocument:
    put:
      summary: Detaches a document from a brand.
      description: Detaches a document from a brand..
      operationId: Branding_DetachDocumentByidBydocumentId
      x-api-path-slug: apibrandingiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The documentId
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Brand
  /api/group/{id}/detachdocument:
    put:
      summary: Detaches a document from a group
      description: Detaches a document from a group.
      operationId: Group_DetachDocumentByidBydocumentId
      x-api-path-slug: apigroupiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the group to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Group
  /api/milestone/{id}/detachdocument:
    put:
      summary: Detaches a document from a milestone
      description: Detaches a document from a milestone.
      operationId: Milestone_DetachDocumentByidBydocumentId
      x-api-path-slug: apimilestoneiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the milestone to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Milestone
  /api/property/{id}/detachdocument:
    put:
      summary: Detaches a document from a property
      description: Detaches a document from a property.
      operationId: Property_DetachDocumentByidBydocumentId
      x-api-path-slug: apipropertyiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the property description to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Property
  /api/role/{id}/detachdescription:
    put:
      summary: Detaches a description from a role
      description: Detaches a description from a role.
      operationId: Role_DetachDescriptionByidBydescriptionId
      x-api-path-slug: apiroleiddetachdescription-put
      parameters:
      - in: query
        name: descriptionId
        description: The id of the description to detach
      - in: path
        name: id
        description: The id of the role to detach the description from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Description
      - From
      - Role
  /api/role/{id}/detachdocument:
    put:
      summary: Detaches a document from a role
      description: Detaches a document from a role.
      operationId: Role_DetachDocumentByidBydocumentId
      x-api-path-slug: apiroleiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the role to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Role
  /api/roomdescription/{id}/detachdocumentfromroom:
    put:
      summary: Detaches a document from a room description room.
      description: Detaches a document from a room description room..
      operationId: RoomDescription_DetachDocumentFromRoomByidBydocumentIdByroomId
      x-api-path-slug: apiroomdescriptioniddetachdocumentfromroom-put
      parameters:
      - in: query
        name: documentId
        description: The document Id
      - in: path
        name: id
        description: The room description Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The room Id
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Room
      - Description
      - Room
  /api/tenancy/{id}/detachdocument:
    put:
      summary: Detaches a document from a tenancy role
      description: Detaches a document from a tenancy role.
      operationId: Tenancy_DetachDocumentByidBydocumentId
      x-api-path-slug: apitenancyiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the role to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Tenancy
      - Role
---