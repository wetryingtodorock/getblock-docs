---
title: bch:settxfee \[POST\] {disallowed}
description: Set the transaction fee per kB for this wallet. Overrides the global-paytxfee command line parameter.Can be deactivated by passing 0 as the fee. In that case automatic feeselection will be used by default.
---

### Parameters


`amount` - numeric or string, required

The transaction fee in BTC/kvB

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "settxfee",
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

