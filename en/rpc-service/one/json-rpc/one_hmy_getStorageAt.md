---
title: one:hmy_getStorageAt \[POST\]
description: Returns the value of a storage position at a specified address.
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
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmy_getStorageAt",
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

