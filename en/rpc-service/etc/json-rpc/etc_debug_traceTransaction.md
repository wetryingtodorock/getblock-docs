---
title: etc:debug_traceTransaction \[POST\] {disallowed}
description: Remix uses debug_traceTransaction to implement debugging. Use theDebugger tab in Remix instead of calling debug_traceTransactiondirectly.Reruns the transaction with the same state as when the transactionexecuted.
---

### Parameters


`transactionHash` - data

Transaction hash.

`Object` - None

request options (all optional and default to false)

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceTransaction",
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

