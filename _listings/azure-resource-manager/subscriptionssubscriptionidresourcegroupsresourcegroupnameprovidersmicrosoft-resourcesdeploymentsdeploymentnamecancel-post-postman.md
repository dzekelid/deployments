{
  "info": {
    "name": "Azure Resource Manager API Cancels a currently running template deployment.",
    "_postman_id": "f239feb7-f3d4-4548-a30e-ce961b64acba",
    "description": "You can cancel a deployment only if the provisioningState is Accepted or Running. After the deployment is canceled, the provisioningState is set to Canceled. Canceling a template deployment stops the currently running template deployment and leaves the resource group partially deployed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "deployments",
      "item": [
        {
          "id": "266f339c-0ac8-4921-bdf8-af2bc5a52bfa",
          "name": "Deployments_Cancel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups/:resourceGroupName/providers/Microsoft.Resources/deployments/:deploymentName/cancel"
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
            "description": "You can cancel a deployment only if the provisioningState is Accepted or Running"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c229bc5d-7ff8-463e-a472-ea170298d9af"
            }
          ]
        }
      ]
    }
  ]
}