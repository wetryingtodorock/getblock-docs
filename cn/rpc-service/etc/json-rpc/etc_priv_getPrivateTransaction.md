---
title: etc:priv_getPrivateTransaction \[POST\] {disallowed}
description: Returns the private transaction if you are a participant, otherwise,null.
---

### Parameters


`data` - None

Transaction hash returned by eea_sendRawTransaction or
eea_sendTransaction.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_getPrivateTransaction",
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

