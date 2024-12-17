---
title: rsk:eth_uninstallFilter \[POST\]
description: Uninstalls a filter with given id. Should always be called when watch isno longer needed. Additonally Filters timeout when they aren’t requestedwith eth_getFilterChanges for a period of time.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_uninstallFilter",
"params": ["0xb"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": false
}
```

