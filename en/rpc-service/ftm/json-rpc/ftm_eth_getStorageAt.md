---
title: ftm:eth_getStorageAt - Fantom
description: Example code for the ftm:eth_getStorageAt json-rpc method. Сomplete guide on how to use ftm:eth_getStorageAt json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - hex string

A 20-byte storage address.

`QUANTITY` - hex string

Integer index of the storage position.

`QUANTITY|TAG` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getStorageAt",
"params": ["0x9EC55d57208cb28a7714A2eA3468bD9d5bB15125", "0x0", "latest"],
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

