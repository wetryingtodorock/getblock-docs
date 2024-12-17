---
title: kcc:eth_coinbase - KuCoin Community Chain
description: Example code for the kcc:eth_coinbase json-rpc method. Сomplete guide on how to use kcc:eth_coinbase json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_coinbase",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x7e5f4552091a69125d5dfcb7b8c2659029395bdf"
}
```

