{
  "info": {
    "name": "Azure API Management API OpenIdConnectProviders Delete",
    "_postman_id": "4707440a-b166-42f1-b72d-e816a91c47d2",
    "description": "Deletes specific OpenID Connect Provider of the API Management service instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "openid connect providers",
      "item": [
        {
          "id": "12956d02-5f5f-4291-8907-e3782c441dec",
          "name": "OpenIdConnectProviders_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/openidConnectProviders/:opid"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "serviceName",
                  "value": "serviceName",
                  "type": "string"
                },
                {
                  "id": "opid",
                  "value": "opid",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "If-Match",
                "value": "{}",
                "description": "The entity state (Etag) version of the OpenID Connect Provider to delete",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes specific OpenID Connect Provider of the API Management service instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aed8cb1e-f3f5-4d9d-92d1-07d9ed6133ad"
            }
          ]
        }
      ]
    }
  ]
}