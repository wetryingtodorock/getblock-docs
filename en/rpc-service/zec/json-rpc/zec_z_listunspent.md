---
title: zec:z_listunspent  {disallowed} - Zcash
description: Example code for the zec:z_listunspent  {disallowed} json-rpc method. Сomplete guide on how to use zec:z_listunspent  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`minconf` - numeric

Optional, default=1

The minimum confirmations to filter.

`maxconf` - numeric

Optional, default=9999999

The maximum confirmations to filter.

`includeWatchonly` - boolean

Optional, default=false

Also include balance in watchonly addresses (see 'importaddress')

`addresses` - string

A json array of zaddrs (both Sprout and Sapling) to filter on. Duplicate
addresses not allowed.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_listunspent",
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

