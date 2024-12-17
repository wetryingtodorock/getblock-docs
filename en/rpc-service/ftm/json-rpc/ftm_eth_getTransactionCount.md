---
title: ftm:eth_getTransactionCount - Fantom
description: Example code for the ftm:eth_getTransactionCount json-rpc method. Сomplete guide on how to use ftm:eth_getTransactionCount json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

20-byte account address.

`quantity|tag` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionCount",
"params": ["0xc94770007dda54cF92009BFF0dE90c06F603a09f", "latest"],
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

