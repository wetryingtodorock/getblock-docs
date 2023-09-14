---
title: bsc:trace_transaction \[WebSocket\]
description: Provides transaction processing of type trace for the specifiedtransaction.
---

### Parameters


`data` - None

Transaction hash

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "trace_transaction",
"params": ["0x4c253746668dca6ac3f7b9bc18248b558a95b5fc881d140872c2dff984d344a7"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method trace_transaction does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

