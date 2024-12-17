---
title: movr:rpc_methods - Moonriver
description: Example code for the movr:rpc_methods json-rpc method. Сomplete guide on how to use movr:rpc_methods json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "rpc_methods",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "methods": [
            "chain_getBlock",
            "chain_getBlockHash",
            "chain_getFinalisedHead",
            "chain_getFinalizedHead",
            "chain_getHead",
            "chain_getHeader",
            "chain_getRuntimeVersion",
            "chain_subscribeAllHeads",
            "chain_subscribeFinalisedHeads",
            "chain_subscribeFinalizedHeads"
        ]
    }
}
```

