---
title: sol:getBlocks - Solana
description: Example code for the sol:getBlocks json-rpc method. Сomplete guide on how to use sol:getBlocks json-rpc in GetBlock.io Web3 documentation.
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
"method": "getBlocks",
"params": [122791100, 122791185, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        122791100,
        122791101,
        122791102,
        122791103,
        122791105,
        122791106,
        122791107,
        122791108,
        122791113,
        122791114,
        122791184,
        122791185
    ]
}
```

