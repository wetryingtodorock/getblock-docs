---
title: ftm:eth_getBlockTransactionCountByHash \[POST\]
description: Returns the number of transactions in the block matching the given blockhash.
---

### Parameters


`data` - hex string

32-byte block hash.

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByHash",
"params": ["0x00033bca0000046700d44a27301783f44016362a31ee066aa2a3ff82350783a9"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x9"
}
```

