---
title: perm_getNodesAllowlist  {disallowed} - Ethereum
description: Example code for the perm_getNodesAllowlist  {disallowed} ws method. Сomplete guide on how to use perm_getNodesAllowlist  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "perm_getNodesAllowlist",
"params": [],
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

