---
title: eth_accounts - Gnosis
description: Example code for the eth_accounts ws method. Сomplete guide on how to use eth_accounts ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_accounts",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        "0x8a4b7469c9c44826334f44561c5e5859a07b0123"
    ]
}
```

