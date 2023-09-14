---
title: sol:getBlockTime \[POST\]
description: Returns the estimated production time of a block.Each validator reports their UTC time to the ledger on a regularinterval by intermittently adding a timestamp to a Vote for a particularblock. A requested blocks time is calculated from the stake-weightedmean of the Vote timestamps in a set of recent blocks recorded on theledger.
---

### Parameters


`block` - u64

block, identified by Slot.

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getBlockTime",
"params": [122791192],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": 1646011316
}
```

