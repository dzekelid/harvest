{
  "info": {
    "name": "Data.gov API Get Harvest Source Ent Jobs",
    "_postman_id": "8358bd0f-7a6c-492d-a7a8-324bf74cff94",
    "description": "List all jobs for a given source",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "harvest",
      "item": [
        {
          "id": "79603a9e-8b18-40eb-8d7f-a2a85475871d",
          "name": "getHarvestSourceEntJobs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "harvest/source/:ident/jobs/"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page_size",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ident",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all jobs for a given source"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23275352-6aea-4b66-9c3f-115f20272953"
            }
          ]
        }
      ]
    }
  ]
}