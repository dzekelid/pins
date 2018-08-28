swagger: "2.0"
x-collection-name: Slack
x-complete: 1
info:
  title: Slack
  description: one-way-to-interact-with-the-slack-platform-is-its-http-rpcbased-web-api-a-collection-of-methods-requiring-oauth-2-0based-user-bot-or-workspace-tokens-blessed-with-related-oauth-scopes-
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pins.add:
    post:
      summary: Pin Item
      description: Pins an item to a channel.
      operationId: pins_add
      x-api-path-slug: pins-add-post
      parameters:
      - in: formData
        name: channel
        description: Channel to pin the item in
      - in: formData
        name: file
        description: File to pin
      - in: formData
        name: file_comment
        description: File comment to pin
      - in: formData
        name: timestamp
        description: Timestamp of the message to pin
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Pins
  /pins.remove:
    post:
      summary: Unpin Item
      description: Un-pins an item from a channel.
      operationId: pins_remove
      x-api-path-slug: pins-remove-post
      parameters:
      - in: formData
        name: channel
        description: Channel where the item is pinned to
      - in: formData
        name: file
        description: File to un-pin
      - in: formData
        name: file_comment
        description: File comment to un-pin
      - in: formData
        name: timestamp
        description: Timestamp of the message to un-pin
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Pins
  /pins.list:
    get:
      summary: List Pins
      description: Lists items pinned to a channel.
      operationId: pins_list
      x-api-path-slug: pins-list-get
      parameters:
      - in: query
        name: channel
        description: Channel to get pinned items for
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Pins