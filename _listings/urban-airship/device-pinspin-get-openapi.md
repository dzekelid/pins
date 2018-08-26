---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Get Device Pins Pin
  description: Gets Device PIN information.
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /device_pins/{pin}:
    put:
      summary: Put Device Pins Pin
      description: Registers a BlackBerry PIN. This is optional, but recommended,
        for BlackBerry push messages. This returns HTTP 201 Created for the first
        registration and 200 OK for any updates. If you wish to include additional
        information about a device pin, for instance an alias or tags, include a JSON
        payload along with this request. Not including one of these keys removes it
        from the device pin.
      operationId: device_pins.pin.put
      x-api-path-slug: device-pinspin-put
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: pin
        description: A BlackBerry PIN
      - in: path
        name: pin
      responses:
        200:
          description: OK
      tags:
      - Device
      - Pins
      - Pin
    get:
      summary: Get Device Pins Pin
      description: Gets Device PIN information.
      operationId: device_pins.pin.get
      x-api-path-slug: device-pinspin-get
      parameters:
      - in: query
        name: pin
        description: A BlackBerry PIN
      - in: path
        name: pin
      responses:
        200:
          description: OK
      tags:
      - Device
      - Pins
      - Pin
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