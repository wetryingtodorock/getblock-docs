---
title: eth_getCode - Ethereum Classic
description: Example code for the eth_getCode json-rpc method. Сomplete guide on how to use eth_getCode json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - integer or string

20-byte contract address.

`QUANTITY|TAG` - string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getCode",
"params": ["0x7eb4c9d6b763324eea4852f5d40985bbf0f29832", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x"
}
```

