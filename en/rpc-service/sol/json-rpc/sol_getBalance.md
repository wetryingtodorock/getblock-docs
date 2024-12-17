---
title: getBalance - Solana
description: Example code for the getBalance json-rpc method. Сomplete guide on how to use getBalance json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Pubkey` - string

Pubkey of account to query, as base-58 encoded string

`Commitment` - object

Optional

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getBalance",
"params": ["83astBRguLMdt2h5U1Tpdq5tjFoJ6noeGwaY3mDLVcri", null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "context": {
            "slot": 123033162
        },
        "value": 0
    }
}
```

