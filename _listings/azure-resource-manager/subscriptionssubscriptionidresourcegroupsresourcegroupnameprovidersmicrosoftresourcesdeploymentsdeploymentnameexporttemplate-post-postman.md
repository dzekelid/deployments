{
  "info": {
    "name": "Azure Resource Manager API Deployments Export Template",
    "_postman_id": "cad76a32-ba5e-4536-a9c3-064eda9aab26",
    "description": "Exports the template used for specified deployment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "deployments",
      "item": [
        {
          "id": "342e0974-b5c8-4702-a747-a4f47d098685",
          "name": "Deployments_ExportTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups/:resourceGroupName/providers/Microsoft.Resources/deployments/:deploymentName/exportTemplate"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Exports the template used for specified deployment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8402757-6b0e-4d71-bf80-9f75d202e15c"
            }
          ]
        }
      ]
    }
  ]
}