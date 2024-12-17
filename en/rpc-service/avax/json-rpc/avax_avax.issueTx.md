---
title: avax:avax.issueTx \[POST\] {disallowed}
description: Send a signed transaction to the network.
---

### Parameters


`tx` - string

transaction

`encoding` - string

Optional.

encoding specifies the format of the signed transaction. Can be either
"cb58" or "hex". Defaults to "cb58".

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "avax.issueTx",
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

