---
title: gno:eth_uninstallFilter \[WebSocket\]
description: Uninstalls a filter with the specified ID. When a filter is no longerrequired, call this method.Filters time out when not requested by eth_getFilterChanges oreth_getFilterLogs for 10 minutes.
---

### Parameters


`data` - hex string

Filter ID.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_uninstallFilter",
"params": ["0x6b08"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": true
}
```

