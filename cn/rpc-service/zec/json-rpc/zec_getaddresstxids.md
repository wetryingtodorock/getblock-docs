---
title: zec:getaddresstxids \[POST\] {disallowed}
description: Returns the txids for given transparent addresses within the given(inclusive) block height range, default is the full blockchain.WARNING getaddresstxids is disabled.
---

### Parameters


`addresses` - list of string

List of the base58check encoded addresses

`start` - number

Optional.

The start block height.

`end` - number

Optional.

The end block height.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddresstxids",
"params": [null, null, null],
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

