{
  "info": {
    "name": "Azure Resource Manager API Policy Definitions Delete",
    "_postman_id": "dd1f038f-6766-4000-b82e-b2ac01e34810",
    "description": "Deletes a policy definition.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "policy definitions",
      "item": [
        {
          "id": "709803dc-d842-4ab6-ab64-9afe80edc395",
          "name": "PolicyDefinitions_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a policy definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13bdf6f3-ab2e-47cf-a836-5d1ab2afddec"
            }
          ]
        }
      ]
    }
  ]
}