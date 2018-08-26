{
  "info": {
    "name": "Google Cloud Deployment Manager Get Deployments",
    "_postman_id": "0ca8753b-888d-4bae-905b-96530d816d99",
    "description": "Lists all deployments for a given project.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Deployment",
      "item": [
        {
          "id": "5dc298ec-825a-47ac-bc6c-a7a8c886cebe",
          "name": "deploymentmanager.deployments.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                ":project/global/deployments"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "project",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all deployments for a given project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cf3ec42-21ed-494c-9813-002a8c8b5dac"
            }
          ]
        }
      ]
    }
  ]
}