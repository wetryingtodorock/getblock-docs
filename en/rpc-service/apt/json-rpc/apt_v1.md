---
title: apt:/v1 - Aptos
description: Example code for the apt:/v1 json-rpc method. Сomplete guide on how to use apt:/v1 json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://apt.getblock.io/v1?' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "block_height": "58851650",
    "chain_id": 1,
    "epoch": "2796",
    "git_hash": "6568c5ee6a58b4f96c0780d4f66d7e573e61c418",
    "ledger_timestamp": "1685696086534090",
    "ledger_version": "152087593",
    "node_role": "full_node",
    "oldest_block_height": "1101178",
    "oldest_ledger_version": "2287593"
}
```

