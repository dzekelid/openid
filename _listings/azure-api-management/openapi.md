swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 1
info:
  title: ApiManagementClient
  description: use-these-rest-apis-for-performing-operations-on-user-entity-in-azure-api-management-deployment--the-user-entity-in-api-management-represents-the-developers-that-call-the-apis-of-the-products-to-which-they-are-subscribed-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/openidConnectProviders
  : get:
      summary: OpenIdConnectProviders ListByService
      description: Lists all OpenID Connect Providers.
      operationId: OpenIdConnectProviders_ListByService
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameopenidconnectproviders-get
      parameters:
      - in: query
        name: $filter
        description: '| Field | Supported operators    | Supported functions                         ||-------|------------------------|---------------------------------------------||
          id    | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith
          || name  | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith
          |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - OpenId Connect Providers
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/openidConnectProviders/{opid}
  : get:
      summary: OpenIdConnectProviders Get
      description: Gets specific OpenID Connect Provider.
      operationId: OpenIdConnectProviders_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameopenidconnectprovidersopid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - OpenId Connect Providers
    put:
      summary: OpenIdConnectProviders CreateOrUpdate
      description: Creates or updates the OpenID Connect Provider.
      operationId: OpenIdConnectProviders_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameopenidconnectprovidersopid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Create parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - OpenId Connect Providers
    patch:
      summary: OpenIdConnectProviders Update
      description: Updates the specific OpenID Connect Provider.
      operationId: OpenIdConnectProviders_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameopenidconnectprovidersopid-patch
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the OpenID Connect Provider
          to update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Update parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - OpenId Connect Providers
    delete:
      summary: OpenIdConnectProviders Delete
      description: Deletes specific OpenID Connect Provider of the API Management
        service instance.
      operationId: OpenIdConnectProviders_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameopenidconnectprovidersopid-delete
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the OpenID Connect Provider
          to delete
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - OpenId Connect Providers