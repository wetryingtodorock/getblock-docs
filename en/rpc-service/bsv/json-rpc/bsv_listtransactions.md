---
title: bsv:listtransactions \[POST\] {disallowed}
description: If a label name is provided, this will return only incoming transactionspaying to addresses with the specified label.Returns up to ‘count’ most recent transactions skipping the first ‘from’transactions.
---

### Parameters


`label` - string, optional

If set, should be a valid label name to return only incoming
transactions with the specified label, or “\*” to disable filtering and
return all transactions.

`count` - numeric, optional, default=10

The number of transactions to return

`skip` - numeric, optional, default=0

The number of transactions to skip

`include_watchonly` - boolean, optional, default=true for watch-only
wallets, otherwise false

Include transactions to watch-only addresses (see ‘importaddress’)

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "listtransactions",
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

