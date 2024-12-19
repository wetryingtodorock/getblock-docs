---
title: eth_getStorageAt - Ethereum Classic
description: Example code for the eth_getStorageAt json-rpc method. Сomplete guide on how to use eth_getStorageAt json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

A 20-byte storage address.

`storage` - string

Integer index of the storage position.

`QUANTITY|TAG` - string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getStorageAt",
"params": ["0x7eb4c9d6b763324eea4852f5d40985bbf0f29832", 0, "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0000000000000000000000000000000000000000000000000000000000000000"
}
```

