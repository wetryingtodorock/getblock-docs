---
title: eth:eth_getFilterChanges \[WebSocket\]
description: Polls the specified filter and returns an array of changes that haveoccurred since the last poll.
---

### Parameters


`data` - None

Filter ID.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0xf8bf5598d9e04fbe84523d42640b9b0e"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "filter not found"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

