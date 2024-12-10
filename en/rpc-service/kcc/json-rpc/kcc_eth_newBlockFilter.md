---
title: kcc:eth_newBlockFilter - KuCoin Community Chain
description: Example code for the kcc:eth_newBlockFilter json-rpc method. Сomplete guide on how to use kcc:eth_newBlockFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newBlockFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x17d41b42a97cd7bf3c77c25a79c49c88"
}
```

