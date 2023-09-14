---
title: neo:listplugins \[POST\]
description: Returns a list of plugins loaded by the node.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "listplugins",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        {
            "interfaces": [],
            "name": "ImportBlocks",
            "version": "2.12.2.0"
        },
        {
            "interfaces": [
                "IPersistencePlugin",
                "IRpcPlugin"
            ],
            "name": "RpcNep5Tracker",
            "version": "2.12.2.0"
        },
        {
            "interfaces": [
                "ILogPlugin",
                "IPolicyPlugin"
            ],
            "name": "SimplePolicyPlugin",
            "version": "2.12.2.0"
        }
    ]
}
```

