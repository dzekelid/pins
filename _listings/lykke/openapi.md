---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/PinSecurity:
    get:
      summary: Get API Pinsecurity
      description: Get api pinsecurity.
      operationId: ApiPinSecurityGet
      x-api-path-slug: apipinsecurity-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: pin
      responses:
        200:
          description: OK
      tags:
      - Pinsecurity
    post:
      summary: Add API Pinsecurity
      description: Add api pinsecurity.
      operationId: ApiPinSecurityPost
      x-api-path-slug: apipinsecurity-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Pinsecurity
---