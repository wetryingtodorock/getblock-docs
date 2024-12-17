---
title: eth:priv_getTransactionReceipt \[POST\] {disallowed}
description: Returns information about the private transaction after mining thetransaction. Receipts for pending transactions are not available.
---

### Parameters


`data` - None

32-byte hash of a transaction.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_getTransactionReceipt",
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

