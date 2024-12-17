---
title: etc:web3_clientVersion - Ethereum Classic
description: Example code for the etc:web3_clientVersion json-rpc method. Сomplete guide on how to use etc:web3_clientVersion json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
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
    "result": "besu/v21.7.2/linux-x86_64/adoptopenjdk-java-11"
}
```

