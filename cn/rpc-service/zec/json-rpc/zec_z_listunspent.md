---
title: zec:z_listunspent \[POST\] {disallowed}
description: Returns array of unspent shielded notes with between minconf and maxconf(inclusive) confirmations.Optionally filter to only include notes sent to specified addresses.When minconf is 0, unspent notes with zero confirmations are returned,even though they are not immediately spendable.
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

