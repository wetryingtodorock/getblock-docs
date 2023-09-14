---
title: doge:listtransactions \[POST\] {disallowed}
description: \-Returnsalistofthelasttransactionsforanaccount.EachtransactionisrepresentedwithaTransactionInfoobject.
---

### Parameters


`account` - string

Optional.

Account to list transactions from. Return transactions from all accounts
if None.

`count` - integer

Number of transactions to return.

`from_` - integer

Skip the first \[from\_\] transactions.

`address` - string

Receive address to consider

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "listtransactions",
"params": [null, 2, 0, null],
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

