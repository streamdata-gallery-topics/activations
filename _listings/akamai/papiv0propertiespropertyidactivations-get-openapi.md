---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 0
info:
  title: Akamai API List a Property&#8217;s Activations
  description: List a Property&#8217;s Activations
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cloudlets/api/v2/origins/currentActivations:
    get:
      summary: List Current Cloudlets Origin Activations
      description: List Current Cloudlets Origin Activations
      operationId: cloudletsapiv2originscurrentactivations
      x-api-path-slug: cloudletsapiv2originscurrentactivations-get
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
      - Activations
  /cloudlets/api/v2/origins/{originId}/activations:
    get:
      summary: List Activations for a Cloudlets Origin
      description: List Activations for a Cloudlets Origin
      operationId: cloudletsapiv2originsoriginidactivations
      x-api-path-slug: cloudletsapiv2originsoriginidactivations-get
      parameters:
      - in: query
        name: originId
        description: Unique identifier for the origin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
      - Activations
    post:
      summary: Activate a Cloudlets Origin Version
      description: Activate a Cloudlets Origin Version
      operationId: cloudletsapiv2originsoriginidactivations
      x-api-path-slug: cloudletsapiv2originsoriginidactivations-post
      parameters:
      - in: query
        name: originId
        description: Unique identifier for the origin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
      - Activations
  /cloudlets/api/v2/policies/{policyId}/activations:
    get:
      summary: List Policy Activations
      description: List Policy Activations
      operationId: cloudletsapiv2policiespolicyidactivationsnetworkpropertyname
      x-api-path-slug: cloudletsapiv2policiespolicyidactivations-get
      parameters:
      - in: query
        name: network
        description: Returns only activations for the selected network, either staging
          or prod
        type: string
      - in: query
        name: policyId
        description: The ID of the policy
        type: string
      - in: query
        name: propertyName
        description: Returns only activations for the selected property
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Policies
      - Activations
      - Network
      - propertyname
  /cloudlets/api/v2/policies/{policyId}/versions/{version}/activations:
    post:
      summary: Activate a Policy Version
      description: Activate a Policy Version
      operationId: cloudletsapiv2policiespolicyidversionsversionactivations
      x-api-path-slug: cloudletsapiv2policiespolicyidversionsversionactivations-post
      parameters:
      - in: query
        name: policyId
        description: The ID of the policy
        type: string
      - in: query
        name: version
        description: The version number of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Policies
      - Versions
      - Activations
  /papi/v0/properties/{propertyId}/activations/:
    get:
      summary: List a Property&#8217;s Activations
      description: List a Property&#8217;s Activations
      operationId: papiv0propertiespropertyidactivationscontractidgroupid
      x-api-path-slug: papiv0propertiespropertyidactivations-get
      parameters:
      - in: query
        name: contractId
        description: Unique identifier for the contract
        type: string
      - in: query
        name: groupId
        description: Unique identifier for the group
        type: string
      - in: query
        name: propertyId
        description: Unique identifier for the property
        type: string
      responses:
        200:
          description: OK
      tags:
      - Papi
      - V0
      - Properties
      - Property
      - Activations
      - Contract
      - group
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