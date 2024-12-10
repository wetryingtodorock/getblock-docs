---
title: one:hmy_getBlockTransactionCountByHash - Harmony
description: Example code for the one:hmy_getBlockTransactionCountByHash json-rpc method. Сomplete guide on how to use one:hmy_getBlockTransactionCountByHash json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

32-byte block hash.

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmy_getBlockTransactionCountByHash",
"params": ["0x910c18611575d42685a4d122a71c9d359a68c3f9786e1ca5a18c27819f8504ff"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x1"
}
```

