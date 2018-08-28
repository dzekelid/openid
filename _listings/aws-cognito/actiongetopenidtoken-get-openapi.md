---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Get Open Id Token
  version: 1.0.0
  description: Gets an OpenID token, using a known Cognito ID.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetOpenIdToken:
    get:
      summary: Get Open Id Token
      description: Gets an OpenID token, using a known Cognito ID.
      operationId: getOpenIdToken
      x-api-path-slug: actiongetopenidtoken-get
      parameters:
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: Logins
        description: A set of optional name-value pairs that map provider names to
          provider tokens
        type: string
      responses:
        200:
          description: OK
      tags:
      - Open ID Token
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