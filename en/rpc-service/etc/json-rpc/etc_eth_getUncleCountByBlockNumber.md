---
title: etc:eth_getUncleCountByBlockNumber - Ethereum Classic
description: Example code for the etc:eth_getUncleCountByBlockNumber json-rpc method. Сomplete guide on how to use etc:eth_getUncleCountByBlockNumber json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

Integer representing either the index of the block within the
blockchain, or one of the string tags latest, earliest, or pending, as
described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockNumber",
"params": ["latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0"
}
```

