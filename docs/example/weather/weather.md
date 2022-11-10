---
title: Weather
descpriton: Sample Workflow to query the weather by Webhook
tags:
  - Workflow²
  - Example
  - Weather
  - Webhook

---

# Weather

Example for a Webhook and reply with the Weather in the City

![Workflow Example](/_images/example/weather.png)


## How to use this workflow

**Instructions**

1. Copy the workflow 
2. Navigate to your Workflow editor
3. Click anywhere in the Workflow² window
4. Paste the code (ctrl + v or cmd + v)






``` Javascript
{
  "nodes": [
    {
      "name": "OpenWeatherMap",
      "type": "WF²-nodes-base.openWeatherMap",
      "position": [
        900,
        300
      ],
      "parameters": {
        "cityName": "={{ $json[\"city\"] }}",
        "language": "en"
      },
      "credentials": {
        "openWeatherMapApi": ""
      },
      "typeVersion": 1
    },
    {
      "name": "Webhook GET",
      "type": "WF²-nodes-base.webhook",
      "position": [
        500,
        300
      ],
      "webhookId": "a31f0bbd-a583-470e-9a1e-29a9ce778122",
      "parameters": {
        "path": "weather",
        "options": {
          "responsePropertyName": "data"
        },
        "responseMode": "lastNode"
      },
      "typeVersion": 1
    },
    {
      "name": "Set City",
      "type": "WF²-nodes-base.set",
      "position": [
        700,
        300
      ],
      "parameters": {
        "values": {
          "string": [
            {
              "name": "city",
              "value": "={{ $json[\"query\"][\"parameter\"] || 'berlin,de' }}"
            }
          ]
        },
        "options": {}
      },
      "typeVersion": 1
    },
    {
      "name": "Create Response",
      "type": "WF²-nodes-base.set",
      "position": [
        1100,
        300
      ],
      "parameters": {
        "values": {
          "string": [
            {
              "name": "data",
              "value": "=It has {{$json[\"main\"][\"temp\"]}}\\xE2\\x84\\x83  and feels like {{$json[\"main\"][\"feels_like\"]}}\\xE2\\x84\\x83  in {{$json[\"name\"]}}"
            }
          ]
        },
        "options": {}
      },
      "typeVersion": 1
    }
  ],
  "connections": {
    "Set City": {
      "main": [
        [
          {
            "node": "OpenWeatherMap",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "Webhook GET": {
      "main": [
        [
          {
            "node": "Set City",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "OpenWeatherMap": {
      "main": [
        [
          {
            "node": "Create Response",
            "type": "main",
            "index": 0
          }
        ]
      ]
    }
  }
}
```
