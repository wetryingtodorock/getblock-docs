---
title: avax:avax.import \[POST\] {disallowed}
description: Finalize the transfer of a non-AVAX or AVAX from the X-Chain to theC-Chain. Before this method is called, you must call the X-Chainsavm.export method with assetID AVAX to initiate the transfer.
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
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "avax.import",
"params": [null, null, null, null, null],
"id": "getblock.io"}'
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

