---
title: clique_discard  {disallowed} - Ethereum
description: Example code for the clique_discard  {disallowed} ws method. Сomplete guide on how to use clique_discard  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

20-byte address of proposed signer.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "clique_discard",
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

