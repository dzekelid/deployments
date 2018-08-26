{
  "info": {
    "name": "Azure Resource Manager API Deployments Get",
    "_postman_id": "dbd8e4d9-7d59-4fc4-9ac4-78e3f19442c4",
    "description": "Gets a deployment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "deployments",
      "item": [
        {
          "id": "b25ef53a-487c-480d-9c3e-49e12645af30",
          "name": "Deployments_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups/:resourceGroupName/providers/Microsoft.Resources/deployments/:deploymentName"
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
                  "id": "deploymentName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a deployment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3df99f4-ff31-4eef-9605-e19560e3ee30"
            }
          ]
        }
      ]
    }
  ]
}