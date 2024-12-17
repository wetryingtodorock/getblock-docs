---
title: etc:priv_getEeaTransactionCount \[POST\] {disallowed}
description: Returns the private transaction count for the specified account andgroup of sender and recipients.
---

### Parameters


`data` - None

Account address.

`data` - None

Base64 encoded Orion address of the sender.

`array of data` - None

Base64 encoded Orion addresses of recipients.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_getEeaTransactionCount",
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

