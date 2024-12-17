---
title: avax.importAVAX  {disallowed} - Avalanche
description: Example code for the avax.importAVAX  {disallowed} ws method. Сomplete guide on how to use avax.importAVAX  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`to` - string

to is the address the AVAX is sent to. It should be in hex format.

`sourceChain` - string

sourceChain is the ID or alias of the chain the AVAX is being imported
from. To import funds from the X-Chain, use "X".

`baseFee` - int

Optional.

baseFee is the base fee that should be used when creating the
transaction. If omitted, a suggested fee will be used.

`username` - string

username is the user that controls the address that transaction will be
sent from.

`password` - string

user password

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "avax.importAVAX",
"params": [null, null, null, null, null],
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

