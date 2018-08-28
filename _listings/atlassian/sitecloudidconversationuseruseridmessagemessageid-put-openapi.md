---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Software Cloud API Edit a message in a direct conversation
  description: Authentication required, with scope participate:conversation
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/user/{userId}:
    get:
      summary: Get a direct conversation of a user
      description: Get a direct conversation of a user.
      operationId: ConversationUserGetHandler
      x-api-path-slug: sitecloudidconversationuseruserid-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: userId
        description: The user Id
      responses:
        200:
          description: OK
      tags:
      - Direct
      - Conversation
      - Of
      - User
  /site/{cloudId}/conversation/user/{userId}/message/{messageId}:
    put:
      summary: Edit a message in a direct conversation
      description: Authentication required, with scope participate:conversation
      operationId: UserMessagePutHandler
      x-api-path-slug: sitecloudidconversationuseruseridmessagemessageid-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: messageId
        description: The ID of the message
      - in: path
        name: userId
        description: The user Id
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Message
      - In
      - Direct
      - Conversation
    delete:
      summary: Delete a message in a direct conversation
      description: Authentication required, with scope participate:conversation
      operationId: UserMessageDeleteHandler
      x-api-path-slug: sitecloudidconversationuseruseridmessagemessageid-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: messageId
        description: The ID of the message
      - in: path
        name: userId
        description: The user Id
      responses:
        200:
          description: OK
      tags:
      - Message
      - In
      - Direct
      - Conversation
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