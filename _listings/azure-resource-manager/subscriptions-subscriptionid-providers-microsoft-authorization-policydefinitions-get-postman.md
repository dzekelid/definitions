{
  "info": {
    "name": "Azure Resource Manager API Policy Definitions List",
    "_postman_id": "21707f12-220f-4f45-b9b7-e53abddae2a4",
    "description": "Gets all the policy definitions for a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "policy definitions",
      "item": [
        {
          "id": "9b6c4671-405d-432a-aff9-cd55aca49dd9",
          "name": "PolicyDefinitions_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Authorization/policydefinitions"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the policy definitions for a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1715ebd6-13a5-4f4e-bb85-7a6f808bcf3f"
            }
          ]
        }
      ]
    }
  ]
}