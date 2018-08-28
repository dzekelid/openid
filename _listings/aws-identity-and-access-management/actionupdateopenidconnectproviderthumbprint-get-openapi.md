---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Update Open I D Connect Provider Thumbprint
  version: 1.0.0
  description: |-
    Replaces the existing list of server certificate thumbprints associated with an OpenID
          Connect (OIDC) provider resource object with a new list of thumbprints.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddClientIDToOpenIDConnectProvider:
    get:
      summary: Add Client I D To Open I D Connect Provider
      description: |-
        Adds a new client ID (also known as audience) to the list of client IDs already
              registered for the specified IAM OpenID Connect (OIDC) provider resource.
      operationId: addClientIDToOpenIDConnectProvider
      x-api-path-slug: actionaddclientidtoopenidconnectprovider-get
      parameters:
      - in: query
        name: ClientID
        description: The client ID (also known as audience) to add to the IAM OpenID
          Connect provider      resource
        type: string
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OpenID Connect (OIDC)
          provider resource to      add the client ID to
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=CreateOpenIDConnectProvider:
    get:
      summary: Create Open I D Connect Provider
      description: Creates an IAM entity to describe an identity provider (IdP) that
        supports.
      operationId: createOpenIDConnectProvider
      x-api-path-slug: actioncreateopenidconnectprovider-get
      parameters:
      - in: query
        name: ClientIDList.member.N
        description: A list of client IDs (also known as audiences)
        type: string
      - in: query
        name: ThumbprintList.member.N
        description: A list of server certificate thumbprints for the OpenID Connect
          (OIDC) identity      providers server certificate(s)
        type: string
      - in: query
        name: Url
        description: The URL of the identity provider
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=DeleteOpenIDConnectProvider:
    get:
      summary: Delete Open I D Connect Provider
      description: Deletes an OpenID Connect identity provider (IdP) resource object
        in IAM.
      operationId: deleteOpenIDConnectProvider
      x-api-path-slug: actiondeleteopenidconnectprovider-get
      parameters:
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OpenID Connect provider
          resource object to      delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=GetOpenIDConnectProvider:
    get:
      summary: Get Open I D Connect Provider
      description: |-
        Returns information about the specified OpenID Connect (OIDC) provider resource object
              in IAM.
      operationId: getOpenIDConnectProvider
      x-api-path-slug: actiongetopenidconnectprovider-get
      parameters:
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the OIDC provider resource
          object in IAM to get      information for
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=ListOpenIDConnectProviders:
    get:
      summary: List Open I D Connect Providers
      description: |-
        Lists information about the IAM OpenID Connect (OIDC) provider resource objects
              defined in the AWS account.
      operationId: listOpenIDConnectProviders
      x-api-path-slug: actionlistopenidconnectproviders-get
      parameters:
      - in: query
        name: OpenIDConnectProviderList.member.N
        description: The list of IAM OIDC provider resource objects defined in the
          AWS      account
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=RemoveClientIDFromOpenIDConnectProvider:
    get:
      summary: Remove Client I D From Open I D Connect Provider
      description: |-
        Removes the specified client ID (also known as audience) from the list of client IDs
              registered for the specified IAM OpenID Connect (OIDC) provider resource object.
      operationId: removeClientIDFromOpenIDConnectProvider
      x-api-path-slug: actionremoveclientidfromopenidconnectprovider-get
      parameters:
      - in: query
        name: ClientID
        description: The client ID (also known as audience) to remove from the IAM
          OIDC provider resource
        type: string
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OIDC provider resource
          to remove the client      ID from
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=UpdateOpenIDConnectProviderThumbprint:
    get:
      summary: Update Open I D Connect Provider Thumbprint
      description: |-
        Replaces the existing list of server certificate thumbprints associated with an OpenID
              Connect (OIDC) provider resource object with a new list of thumbprints.
      operationId: updateOpenIDConnectProviderThumbprint
      x-api-path-slug: actionupdateopenidconnectproviderthumbprint-get
      parameters:
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OIDC provider resource
          object for which you      want to update the thumbprint
        type: string
      - in: query
        name: ThumbprintList.member.N
        description: A list of certificate thumbprints that are associated with the
          specified IAM OpenID      Connect provider
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
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