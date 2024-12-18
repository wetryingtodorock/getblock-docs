---
title: eth_getLogs - Ethereum Classic
description: Example code for the eth_getLogs json-rpc method. Сomplete guide on how to use eth_getLogs json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - json object

Filter options object.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getLogs",
"params": [{"fromBlock": "earliest", "toBlock": "latest", "address": "0x7eb4c9d6b763324eea4852f5d40985bbf0f29832", "topics": []}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": []
}
```

