---
title: eth_sign  {disallowed} - Avalanche
description: Example code for the eth_sign  {disallowed} ws method. Сomplete guide on how to use eth_sign  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address.

`DATA` - string

message to sign.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0x0f8d94cea1eba9c582bbe800545ca91dfc39da18", "0xdeadbeaf"],
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

