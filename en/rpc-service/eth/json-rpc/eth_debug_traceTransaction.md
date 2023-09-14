---
title: eth:debug_traceTransaction \[POST\] {disallowed}
description: Remix uses debug_traceTransaction to implement debugging. Use theDebugger tab in Remix instead of calling debug_traceTransactiondirectly.Reruns the transaction with the same state as when the transactionexecuted.
---

### Parameters


`transactionHash` - data

Transaction hash.

`Object` - None

request options (all optional and default to false)

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceTransaction",
"params": ["0xcd718a69d478340dc28fdf6bf8056374a52dc95841b44083163ced8dfe29310c", null],
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

