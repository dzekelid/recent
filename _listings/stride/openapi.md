---
swagger: "2.0"
x-collection-name: Stride
x-complete: 1
info:
  title: Stride
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
host: api.atlassian.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/{conversationId}/message/recent:
    get:
      summary: Get latest messages for conversation
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationMessageRecentByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationidmessagerecent-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: query
        name: limit
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Message
      - Recent
---