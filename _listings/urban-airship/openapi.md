---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 1
info:
  title: Urban Airship
  description: the-urban-airships-api-powers-mobile-applications-with-push-rich-push-inapp-purchases-and-subscription-services-
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
    delete:
      summary: Delete Device Pins Pin
      description: Marks a PIN as inactive. No notifications will be delivered to
        it until a PUT is executed again.
      operationId: device_pins.pin.delete
      x-api-path-slug: device-pinspin-delete
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
---