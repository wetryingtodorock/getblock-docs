---
title: masternode_count - Dash
description: Example code for the masternode_count json-rpc method. Сomplete guide on how to use masternode_count json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`method name` - string

None

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "masternode",
"params": ["count"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "enabled": 4630,
        "total": 4873
    }
}
```

