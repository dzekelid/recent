{
  "info": {
    "name": "Steem get recent categories",
    "_postman_id": "ddd5d3f7-fb51-4326-9f3c-8cf486b1e3d5",
    "description": "get tags",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "2900579b-eeb5-43e0-ab93-eb9a4ad735d2",
          "name": "get-tags",
          "request": {
            "url": "http://api.steemjs.com/get_active_categories?after=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b83af85-a2fb-43b1-b591-fc7918706468"
            }
          ]
        },
        {
          "id": "7824aad5-8f7f-40ed-ac5f-d72e088a778e",
          "name": "get-tags1",
          "request": {
            "url": "http://api.steemjs.com/get_best_categories?after=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4c3b3f9-c0b8-4990-918e-8714dab63457"
            }
          ]
        },
        {
          "id": "a1233b81-29d8-4a20-9a0c-edce08018fb0",
          "name": "get-tags2",
          "request": {
            "url": "http://api.steemjs.com/get_recent_categories?after=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30fcabec-035d-432d-a4bd-1b4487ceb3a7"
            }
          ]
        }
      ]
    }
  ]
}