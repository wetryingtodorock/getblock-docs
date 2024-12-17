---
title: mnr_getWork - Rootstock
description: Example code for the mnr_getWork ws method. Сomplete guide on how to use mnr_getWork ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "mnr_getWork",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method mnr_getWork does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

