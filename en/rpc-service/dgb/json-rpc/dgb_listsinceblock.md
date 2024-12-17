---
title: dgb:listsinceblock \[POST\] {disallowed}
description: Get all transactions in blocks since block \[blockhash\], or alltransactions if omitted.If “blockhash” is no longer a part of the main chain, transactions fromthe fork point onward are included.Additionally, if include_removed is set, transactions affecting thewallet which were removed are returned in the “removed” array.
---

### Parameters


`blockhash` - string, optional

If set, the block hash to list transactions since, otherwise list all
transactions.

`target_confirmations` - numeric, optional, default=1

Return the nth block hash from the main chain. e.g. 1 would mean the
best block hash.

Note this is not used as a filter, but only affects \[lastblock\] in the
return value

`include_watchonly` - boolean, optional, default=true for watch-only
wallets, otherwise false

Include transactions to watch-only addresses (see ‘importaddress’)

`include_removed` - boolean, optional, default=true

Show transactions that were removed due to a reorg in the “removed”
array (not guaranteed to work on pruned nodes)

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "listsinceblock",
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

