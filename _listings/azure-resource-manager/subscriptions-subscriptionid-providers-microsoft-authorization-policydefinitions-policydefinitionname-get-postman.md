{
  "info": {
    "name": "Azure Resource Manager API Policy Definitions Get",
    "_postman_id": "a56979a5-8fa7-43ae-8e76-6840b481a289",
    "description": "Gets the policy definition.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "policy definitions",
      "item": [
        {
          "id": "4700084d-ceff-4b7b-aa10-e333a249e18c",
          "name": "PolicyDefinitions_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Authorization/policydefinitions/:policyDefinitionName"
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
                  "id": "policyDefinitionName",
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
            "description": "Gets the policy definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92c2ee01-9488-49f8-9b56-79eac9acb51e"
            }
          ]
        }
      ]
    }
  ]
}