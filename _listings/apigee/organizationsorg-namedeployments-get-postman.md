{
  "info": {
    "name": "Apigee Edge Get Organizations Name Deployments",
    "_postman_id": "c3eb9cce-6864-4d6d-91dc-d2edd8289c4a",
    "description": "Gets all deployments of an organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "a1787980-6202-4ade-98b6-94fce5861c56",
          "name": "getOrganizationsOrgNameDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/deployments"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all deployments of an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9503647-5488-486d-a53b-d61e57975468"
            }
          ]
        }
      ]
    }
  ]
}