{
  "info": {
    "name": "Azure API Management API OpenIdConnectProviders ListByService",
    "_postman_id": "4c912842-80aa-4a22-865f-15585d722a20",
    "description": "Lists all OpenID Connect Providers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "openid connect providers",
      "item": [
        {
          "id": "ef5eb728-6b07-4b14-8c2f-4c75ee9d57d2",
          "name": "OpenIdConnectProviders_ListByService",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/openidConnectProviders"
              ],
              "query": [
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all OpenID Connect Providers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a270e729-628b-4fdd-9c46-3447a5d42c64"
            }
          ]
        }
      ]
    }
  ]
}