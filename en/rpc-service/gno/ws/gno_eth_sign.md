---
title: gno:eth_sign  {disallowed} - Gnosis
description: Example code for the gno:eth_sign  {disallowed} ws method. Сomplete guide on how to use gno:eth_sign  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - hex string

20 Bytes - address

`DATA` - hex string

N Bytes - message to sign

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0xcee8ae756461e2653b88aefdbd70c1144de52b23", "0xbcda"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

