---
title: eth_getBlockTransactionCountByNumber - Ethereum
description: Example code for the eth_getBlockTransactionCountByNumber json-rpc method. Сomplete guide on how to use eth_getBlockTransactionCountByNumber json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByNumber",
"params": ["0x52A8CA"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x49"
}
```

