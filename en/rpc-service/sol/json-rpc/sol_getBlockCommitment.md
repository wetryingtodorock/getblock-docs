---
title: sol:getBlockCommitment \[POST\]
description: Returns commitment for particular block
---

### Parameters


`block` - u64

block, identified by Slot

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getBlockCommitment",
"params": [122791192],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "commitment": null,
        "totalStake": 388997198076741924
    }
}
```

