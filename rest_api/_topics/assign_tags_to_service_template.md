#### Assigning Tags to a Service Template

##### Request:

    POST /api/service_templates/1/tags

``` json
{
  "action" : "assign",
  "resources" : [
    { "category" : "location", "name" : "ny" },
    { "category" : "department", "name" : "finance" }
  ]
}
```

##### Response:

``` json
{
  "results": [
    {
      "success": true,
      "message": "Assigning Tag: category:'location' name:'ny'",
      "href": "https://hostname/api/service_templates/1",
      "tag_category": "location",
      "tag_name": "ny"
    },
    {
      "success": true,
      "message": "Assigning Tag: category:'department' name:'finance'",
      "href": "https://hostname/api/service_templates/1",
      "tag_category": "department",
      "tag_name": "finance"
    }
  ]
}
```
