---
title: getBlocksWithLimit - Solana
description: Example code for the getBlocksWithLimit json-rpc method. Сomplete guide on how to use getBlocksWithLimit json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`start_slot` - u64

first slot, as u64 integer

`end_slot` - u64

Optional.

last slot, as u64 integer

`commitment` - object

Optional.

"processed" is not supported. If parameter not provided, the default is
"finalized".

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getBlocksWithLimit",
"params": [5, 10, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        122257143,
        122257144,
        122257145,
        122257146,
        122257147,
        122257148,
        122257149,
        122257150,
        122257151,
        122257152
    ]
}
```

