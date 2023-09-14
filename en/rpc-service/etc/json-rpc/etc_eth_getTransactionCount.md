---
title: etc:eth_getTransactionCount \[POST\]
description: Returns the number of transactions sent from a specified address. Usethe pending tag to get the next account nonce not used by any pendingtransactions.
---

### Parameters


`data` - string

20-byte account address.

`quantity|tag` - string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionCount",
"params": ["0x7eb4c9d6b763324eea4852f5d40985bbf0f29832", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x22c"
}
```

