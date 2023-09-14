---
title: neo:getpeers \[POST\]
description: Gets a list of nodes that the node is currently connected/disconnectedfrom.Response Description\- Unconnected Nodes that are not currently connected.\- Bad Nodes that are no longer connected.\- Connected Nodes to which you are currently connected.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getpeers",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "bad": [],
        "connected": [
            {
                "address": "13.251.207.0",
                "port": 10333
            },
            {
                "address": "104.43.136.59",
                "port": 10333
            },
            {
                "address": "13.82.50.205",
                "port": 10333
            }
        ],
        "unconnected": [
            {
                "address": "144.76.0.7",
                "port": 10333
            },
            {
                "address": "91.149.225.131",
                "port": 10333
            },
            {
                "address": "67.189.155.247",
                "port": 10333
            }
        ]
    }
}
```

