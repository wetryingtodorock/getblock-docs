---
title: zec:z_mergetoaddress \[POST\] {disallowed}
description: Merge multiple UTXOs and notes into a single UTXO or note. CoinbaseUTXOs are ignored use \`z_shieldcoinbase\` to combine those into asingle note.This is an asynchronous operation, and UTXOs selected for merging willbe locked. If there is an error, they are unlocked. The RPC call\`listlockunspent\` can be used to return a list of locked UTXOs.The number of UTXOs and notes selected for merging can be limited by thecaller. If the transparent limit parameter is set to zero will meanlimit the number of UTXOs based on the size of the transaction. Anylimit is constrained by the consensus rule defining a maximumtransaction size of 100000 bytes before Sapling, and 2000000 bytes onceSapling activates.
---

### Parameters


`fromaddresses` - array

A JSON array with addresses.

While it is possible to use a variety of different combinations of
addresses and the above values, it is not possible to send funds from
both sprout and sapling addresses simultaneously. If a special string is
given, any given addresses of that type will be counted as duplicates
and cause an error.

`toaddress` - string

The taddr or zaddr to send the funds to.

`fee` - numeric

Optional, default=0.00001

The fee amount to attach to this transaction.

`transparent_limit` - numeric

Optional, default=50

Limit on the maximum number of UTXOs to merge. Set to 0 to use as many
as will fit in the transaction.

`shielded_limit` - numeric

Optional, default is 20 Sprout or 200 Sapling Notes

Limit on the maximum number of notes to merge. Set to 0 to merge as many
as will fit in the transaction.

`memo` - string

Optional

Encoded as hex. When toaddress is a zaddr, this will be stored in the
memo field of the new note.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_mergetoaddress",
"params": [null, null, null, null, null, null],
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

