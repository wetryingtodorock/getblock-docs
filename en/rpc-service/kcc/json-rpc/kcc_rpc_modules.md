---
title: kcc:rpc_modules - KuCoin Community Chain
description: Example code for the kcc:rpc_modules json-rpc method. Сomplete guide on how to use kcc:rpc_modules json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "rpc_modules",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "debug": "1.0",
        "eth": "1.0",
        "net": "1.0",
        "rollup": "1.0",
        "rpc": "1.0",
        "web3": "1.0"
    }
}
```

