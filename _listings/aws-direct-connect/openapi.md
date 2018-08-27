---
swagger: "2.0"
x-collection-name: AWS Direct Connect
x-complete: 1
info:
  title: AWS Direct Connect API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateConnection:
    get:
      summary: Create Connection
      description: Creates a new connection between the customer network and a specific
        AWS Direct Connect location.
      operationId: createConnection
      x-api-path-slug: actioncreateconnection-get
      parameters:
      - in: query
        name: bandwidth
        description: Bandwidth of the connection
        type: string
      - in: query
        name: connectionName
        description: The name of the connection
        type: string
      - in: query
        name: location
        description: Where the connection is located
        type: string
      responses:
        200:
          description: OK
      tags:
      - Connections
  /?Action=CreateInterconnect:
    get:
      summary: Create Interconnect
      description: Creates a new interconnect between a AWS Direct Connect partner's
        network and a specific AWS Direct Connect location.
      operationId: createInterconnect
      x-api-path-slug: actioncreateinterconnect-get
      parameters:
      - in: query
        name: bandwidth
        description: The port bandwidth
        type: string
      - in: query
        name: interconnectName
        description: The name of the interconnect
        type: string
      - in: query
        name: location
        description: Where the interconnect is located
        type: string
      responses:
        200:
          description: OK
      tags:
      - Interconnects
  /?Action=DescribeLocations:
    get:
      summary: Describe Locations
      description: Returns the list of AWS Direct Connect locations in the current
        AWS region.
      operationId: describeLocations
      x-api-path-slug: actiondescribelocations-get
      parameters:
      - in: query
        name: locations
        description: A list of colocation hubs where network providers have equipment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Locations
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Describes the tags associated with the specified Direct Connect
        resources.
      operationId: describeTags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: resourceArns
        description: The Amazon Resource Names (ARNs) of the Direct Connect resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=TagResource:
    get:
      summary: Tag Resource
      description: Adds the specified tags to the specified Direct Connect resource.
      operationId: tagResource
      x-api-path-slug: actiontagresource-get
      parameters:
      - in: query
        name: resourceArn
        description: The Amazon Resource Name (ARN) of the Direct Connect resource
        type: string
      - in: query
        name: tags
        description: The list of tags to add
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=UntagResource:
    get:
      summary: Untag Resource
      description: Removes one or more tags from the specified Direct Connect resource.
      operationId: untagResource
      x-api-path-slug: actionuntagresource-get
      parameters:
      - in: query
        name: resourceArn
        description: The Amazon Resource Name (ARN) of the Direct Connect resource
        type: string
      - in: query
        name: tagKeys
        description: The list of tag keys to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
---