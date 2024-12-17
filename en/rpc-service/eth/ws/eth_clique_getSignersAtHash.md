---
title: eth:clique_getSignersAtHash  {disallowed} - Ethereum
description: Example code for the eth:clique_getSignersAtHash  {disallowed} ws method. Сomplete guide on how to use eth:clique_getSignersAtHash  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

32-byte block hash.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "clique_getSignersAtHash",
"params": [null],
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

