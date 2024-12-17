---
title: debug_accountRange  {disallowed} - Ethereum
description: Example code for the debug_accountRange  {disallowed} ws method. Сomplete guide on how to use debug_accountRange  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`blockNrOrHash` - DATA

block number or hash

`DATA` - DATA

start hashed address

`DATA` - int

max results per page

`DATA` - bool

None

`DATA` - bool

None

`DATA` - bool

If incompletes is false, then accounts for which the key preimage (i.e:
the address) doesn’t exist in db are skipped.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_accountRange",
"params": ["0xc48fb64230a82f65a08e7280bd8745e7fea87bc7c206309dee32209fe9a985f7", "0x0f", 0, false, false, false],
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

