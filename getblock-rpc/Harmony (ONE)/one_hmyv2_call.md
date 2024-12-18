---
title: hmyv2_call - Harmony
description: Example code for the hmyv2_call json-rpc method. Сomplete guide on how to use hmyv2_call json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`OBJECT` - None

Transaction call object.

`QUANTITY|TAG` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmyv2_call",
"params": [{"to": "0x69498dd54bd25aa0c886cf1f8b8ae0856d55ff13", "value": "0x1"}, "latest"],
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

