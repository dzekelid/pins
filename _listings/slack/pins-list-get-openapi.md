---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack List Pins
  description: Lists items pinned to a channel.
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