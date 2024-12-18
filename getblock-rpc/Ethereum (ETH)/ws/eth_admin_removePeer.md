---
title: admin_removePeer  {disallowed} - Ethereum
description: Example code for the admin_removePeer  {disallowed} ws method. Сomplete guide on how to use admin_removePeer  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`string` - None

Enode URL of peer to remove.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin_removePeer",
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

