{
  "info": {
    "name": "Data.gov API Get Harvest Sources",
    "_postman_id": "e86a27b7-a705-4cec-9e63-b4761cfb7721",
    "description": "List all harvest sources",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "harvest",
      "item": [
        {
          "id": "1f23c287-4af7-4d8b-9362-029062162c94",
          "name": "getHarvestSources",
          "request": {
            "url": "http://catalog.data.gov/api/3/harvest/sources/?owner=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all harvest sources"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90597b01-7d9f-4314-aafb-c16f72b4d5a6"
            }
          ]
        }
      ]
    }
  ]
}