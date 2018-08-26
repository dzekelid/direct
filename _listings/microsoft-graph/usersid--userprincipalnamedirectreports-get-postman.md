{
  "info": {
    "name": "Microsoft Graph API List Direct Reports",
    "_postman_id": "2bd66816-d04f-4acd-ad16-2f0a174f847d",
    "description": "List directReports Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "adc91f23-1e40-459c-9cb9-aedad8d9d8ff",
          "name": "ListDirectReports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/directReports"
              ],
              "variable": [
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List directReports Get user's direct reports"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "66854d7f-036a-480a-a9ff-dac474e6ae40"
            }
          ]
        }
      ]
    }
  ]
}