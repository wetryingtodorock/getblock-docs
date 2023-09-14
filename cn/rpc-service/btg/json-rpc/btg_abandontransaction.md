---
title: btg:abandontransaction \[POST\] {disallowed}
description: Mark in-wallet transaction txid as abandonedThis will mark this transaction and all its in-wallet descendants asabandoned which will allow for their inputs to be respent. It can beused to replace stuck or evicted transactions.It only works on transactions which are not included in a block and arenot currently in the mempool.It has no effect on transactions which are already abandoned.
---

### Parameters


`txid` - string, required

The transaction id

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "abandontransaction",
"params": [null],
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

