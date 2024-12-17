---
title: cro:web3_clientVersion - Cronos
description: Example code for the cro:web3_clientVersion json-rpc method. Сomplete guide on how to use cro:web3_clientVersion json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
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
    "result": "Version dev ()\nCompiled at  using Go go1.19.6 (amd64)"
}
```

