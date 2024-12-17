---
title: eth_getLogs - Ethereum
description: Example code for the eth_getLogs json-rpc method. Сomplete guide on how to use eth_getLogs json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - None

Filter options object.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getLogs",
"params": [{"fromBlock": "0x107D7B0", "toBlock": "0x107D7B0", "address": "0x901c7C311d39e0b26257219765E71E8DB3107A81", "topics": []}],
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

