---
title: kcc:web3_clientVersion - KuCoin Community Chain
description: Example code for the kcc:web3_clientVersion json-rpc method. Сomplete guide on how to use kcc:web3_clientVersion json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "web3_clientVersion",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "Geth/v1.9.10-stable/linux-amd64/go1.15.15"
}
```

