---
title: ftm:web3_clientVersion - Fantom
description: Example code for the ftm:web3_clientVersion json-rpc method. Сomplete guide on how to use ftm:web3_clientVersion json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
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
    "result": "go-opera/v1.1.2-rc.6-9bacdc25-1678723432/linux-amd64/go1.18.10"
}
```

