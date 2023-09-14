---
title: fuse:eth_sendRawTransaction \[WebSocket\]
description: Creates new message call transaction or a contract creation for signedtransactions.
---

### Parameters


`DATA` - string

The signed transaction data.

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_sendRawTransaction",
"params": ["0xd46e8dd67c5d32be8d46e8dd67c5d32be8058bb8eb970870f072445675058bb8eb970870f072445675"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32602,
        "data": "RlpIncorrectListLen",
        "message": "Invalid RLP."
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

