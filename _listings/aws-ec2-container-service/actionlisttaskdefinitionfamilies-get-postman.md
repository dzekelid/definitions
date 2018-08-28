{
  "info": {
    "name": "Amazon EC2 Container Service API List Task Definition Families",
    "_postman_id": "95f31516-be84-4de1-aa68-63d52f325913",
    "description": "Returns a list of task definition families that are registered to your account\n            (which may include task definition families that no longer have any ACTIVE\n            task definition revisions).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Task Definitions",
      "item": [
        {
          "id": "4e60b862-5331-4f21-8c3a-85add4b1e535",
          "name": "deregisterTaskDefinition",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskDefinition?taskDefinition=taskDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters the specified task definition by family and revision."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bc4acc3-4110-4235-b279-92eb0c3ba38e"
            }
          ]
        },
        {
          "id": "27dca945-8abd-4719-b3bd-07009cc55998",
          "name": "describeTaskDefinition",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTaskDefinition?taskDefinition=taskDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a task definition."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9ab3926-97fc-4a4f-8ebd-bf5b23d6bd87"
            }
          ]
        }
      ]
    },
    {
      "name": "Tasks",
      "item": [
        {
          "id": "3eec2ea6-21e5-4253-ae94-3dbde9cf9c2a",
          "name": "describeTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTasks?cluster=cluster&tasks=tasks",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a specified task or tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa59779a-efca-491a-aa3d-922127081eec"
            }
          ]
        }
      ]
    },
    {
      "name": "Task Definition Families",
      "item": [
        {
          "id": "b3fb4f4f-5edd-4141-afc2-e4229fdda70f",
          "name": "listTaskDefinitionFamilies",
          "request": {
            "url": "http://example.com/api/?Action=ListTaskDefinitionFamilies?familyPrefix=familyPrefix&maxResults=maxResults&nextToken=nextToken&status=status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of task definition families that are registered to your account\n            (which may include task definition families that no longer have any ACTIVE\n            task definition revisions)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "911b1b09-ec63-4403-910d-94c670080168"
            }
          ]
        }
      ]
    }
  ]
}