---
title: zec:z_shieldcoinbase \[POST\] {disallowed}
description: Shield transparent coinbase funds by sending to a shielded zaddr. Thisis an asynchronous operation and utxos selected for shielding will belocked. If there is an error, they are unlocked. The RPC call\`listlockunspent\` can be used to return a list of locked utxos. Thenumber of coinbase utxos selected for shielding can be limited by thecaller. Any limit is constrained by the consensus rule defining amaximum transaction size of 100000 bytes before Sapling, and 2000000bytes once Sapling activates.
---

### Parameters


`fromaddresses` - string

The address is a taddr or "\*" for all taddrs belonging to the wallet.

`toaddresses` - string

The address is a zaddr.

`fee` - numeric

Optional, default=0.00001

The fee amount to attach to this transaction.

`limit` - numeric

Optional, default=50

Limit on the maximum number of utxos to shield. Set to 0 to use as many
as will fit in the transaction.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_shieldcoinbase",
"params": [null, null, null, null],
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

