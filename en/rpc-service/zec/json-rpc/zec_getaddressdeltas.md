---
title: zec:getaddressdeltas \[POST\] {disallowed}
description: Returns all changes for an address.Returns information about all changes to the given transparent addresseswithin the given (inclusive) block height range, default is the fullblockchain.WARNING getaddressdeltas is disabled.
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

`chainInfo` - boolean

Optional, default=false

Include chain info in results, only applies if start and end specified.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddressdeltas",
"params": [null, null, null, null],
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

