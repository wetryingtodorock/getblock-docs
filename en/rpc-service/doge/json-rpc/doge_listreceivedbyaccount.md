---
title: doge:listreceivedbyaccount \[POST\] {disallowed}
description: \-Returnsalistofaccounts.EachaccountisrepresentedwithaAccountInfoobject.
---

### Parameters


`minconf` - integer

Minimum number of confirmations before payments are included.

`includeempty` - boolean

Optional, default=false

Whether to include addresses that haven’t received any payments.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "listreceivedbyaccount",
"params": [1, false],
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

