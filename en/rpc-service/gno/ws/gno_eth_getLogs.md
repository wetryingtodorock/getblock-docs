---
title: gno:eth_getLogs \[WebSocket\]
description: Returns an array of logs matching a specified filter object.Leave the --auto-log-bloom-caching-enabled command line option at thedefault value of true to improve log retrieval performance.
---

### Parameters


`Object` - hex string

Filter options object.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getLogs",
"params": [{"fromBlock": "0x1B13C84", "toBlock": "0x1B13C84", "address": "0xe9e7cea3dedca5984780bafc599bd69add087d56", "topics": []}],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32001,
        "message": "28392580 could not be found"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

