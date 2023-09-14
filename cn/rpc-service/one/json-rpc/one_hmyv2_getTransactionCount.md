---
title: one:hmyv2_getTransactionCount \[POST\]
description: Returns the number of transactions sent from a specified address. Usethe pending tag to get the next account nonce not used by any pendingtransactions.
---

### Parameters


`data` - hex string

20-byte account address.

`quantity|tag` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmyv2_getTransactionCount",
"params": ["one1qku72aj98fskvge07h9j0gtfu9sdw62ucgff67", "0x286AC07"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "missing trie node d415596d6e84fb80bcce0cb183592969547169aac226fc8e58c4de28d38d9d5c (path )"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

