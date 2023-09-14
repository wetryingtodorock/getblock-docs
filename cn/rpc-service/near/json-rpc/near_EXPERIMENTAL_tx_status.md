---
title: near:EXPERIMENTAL_tx_status \[POST\] {disallowed}
description: Queries status of a transaction by hash, returning the final transactionresult and details of all receipts.
---

### Parameters


`hash` - string

transaction hash

`id` - string

sender account id, used to determine which shard to query for
transaction.

### Request

``` java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "EXPERIMENTAL_tx_status",
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

