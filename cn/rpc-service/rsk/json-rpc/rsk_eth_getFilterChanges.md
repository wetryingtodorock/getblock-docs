---
title: rsk:eth_getFilterChanges \[POST\]
description: Polling method for a filter, which returns an array of logs whichoccurred since last poll.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0x16"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```

