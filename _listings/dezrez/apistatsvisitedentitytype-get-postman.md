{
  "info": {
    "name": "Dezrez Get all recent history of 'pages' visited on Rezi for a given entity type.",
    "_postman_id": "d9a7d18b-435b-4dc7-8888-70b1196f81a3",
    "description": "Get all recent history of 'pages' visited on rezi for a given entity type..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recent",
      "item": [
        {
          "id": "9c7c2927-9558-47e3-91b5-59d35aefe924",
          "name": "Stats_VisitedByentityType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/stats/visited/:entityType"
              ],
              "variable": [
                {
                  "id": "entityType",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all recent history of 'pages' visited on rezi for a given entity type.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a405521a-f40b-4a1b-b00c-d5894ce6485a"
            }
          ]
        }
      ]
    }
  ]
}