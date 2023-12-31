---
title: zec:prioritisetransaction \[POST\] {disallowed}
description: Accepts the transaction into mined blocks at a higher (or lower)priority
---

### Parameters


`txid` - string

The transaction id.

`priority delta` - numeric

The priority to add or subtract.

The transaction selection algorithm considers the tx as it would have a
higher priority.

(priority of a transaction is calculated: coinage \* value_in_satoshis /
txsize)

`fee delta` - numeric

The fee value (in satoshis) to add (or subtract, if negative).

The fee is not actually paid, only the algorithm for selecting
transactions into a block considers the transaction as it would have
paid a higher (or lower) fee.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "prioritisetransaction",
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

