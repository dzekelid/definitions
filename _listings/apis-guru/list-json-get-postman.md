{
  "info": {
    "name": "APIs.guru List all APIs",
    "_postman_id": "8e1f3bcf-78ed-4642-968f-50d7936fc067",
    "description": "List all APIs in the directory.\nReturns links to OpenAPI specification for each API in the directory.\nIf API exist in multiple versions `preferred` one is explicitly marked.\n\nSome basic info from OpenAPI spec is cached inside each object.\nThis allows to generate some simple views without need to fetch OpenAPI spec for each API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "APIs",
      "item": [
        {
          "id": "3e12b4cd-a5f7-456d-9ae1-d3a73352f399",
          "name": "listAPIs",
          "request": {
            "url": "http://api.apis.guru/v2/list.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all APIs in the directory.\nReturns links to OpenAPI specification for each API in the directory.\nIf API exist in multiple versions `preferred` one is explicitly marked.\n\nSome basic info from OpenAPI spec is cached inside each object.\nThis allows to generate some simple views without need to fetch OpenAPI spec for each API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71a382e1-3ac6-4639-8e7c-63634ccbd1a3"
            }
          ]
        }
      ]
    }
  ]
}