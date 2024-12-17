---
title: dash:/getutxos/{checkmempool}/{txid-n}{format} \[GET\]
description: The GET getutxos operation returns an UTXO set given a set of outpoints.
---

### Parameters


`checkmempool` - path

string, optional 1 or 0

Set to checkmempool to include transactions that are currently in the
memory pool to the calculation

`txid-n` - path

vector, required 1 or more

The list of outpoints to be queried. Each outpoint is the TXID of the
transaction, encoded as hex in RPC byte order with an additional -n
parameter for the output index (vout) number, with the index starting
from 0

`format` - path

required exactly 1

Set to .json for decoded block contents in JSON, or .bin or .hex for a
serialized block in binary or hex

### Request

``` java
curl --location --request GET 'https://dash.getblock.io/mainnet/getutxos/964eb02db9742533bc669d0202c557337bc194786f682d69ef9688f3011497e2-0/964eb02db9742533bc669d0202c557337bc194786f682d69ef9688f3011497e2-0.json' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "bitmap": "00",
    "chainHeight": 1891101,
    "chaintipHash": "000000000000001d507d43a6567386e443deecbe1922f2e4b11bcd0ccb401ada",
    "utxos": []
}
```

