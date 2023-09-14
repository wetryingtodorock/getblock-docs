---
title: dash:submitblock \[POST\] {disallowed}
description: Accepts a block, verifies it is a valid addition to the block chain, andbroadcasts it to the network.Extra parameters are ignored by Dash Core but may be used by miningpools or other programs.
---

### Parameters


`Block` - string (hex)

The full block to submit in serialized block format as hex.

`dummy` - object

Optional.

A dummy value for compatibility with BIP22. This value is ignored.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "submitblock",
"params": [null, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

