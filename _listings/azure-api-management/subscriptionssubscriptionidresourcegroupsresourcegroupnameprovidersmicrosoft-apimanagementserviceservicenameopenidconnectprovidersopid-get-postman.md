{
  "info": {
    "name": "Azure API Management API OpenIdConnectProviders Get",
    "_postman_id": "0d3d1c81-1857-48ee-a2d8-5b86503621e7",
    "description": "Gets specific OpenID Connect Provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "openid connect providers",
      "item": [
        {
          "id": "2cf2c695-6422-457c-a986-b07690e28291",
          "name": "OpenIdConnectProviders_Get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets specific OpenID Connect Provider"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9224898f-dca1-4b24-9ec3-466a0b4b1af3"
            }
          ]
        }
      ]
    }
  ]
}