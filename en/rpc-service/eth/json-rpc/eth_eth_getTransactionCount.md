---
title: eth:eth_getTransactionCount \[POST\]
description: Returns the number of transactions sent from a specified address. Usethe pending tag to get the next account nonce not used by any pendingtransactions.
---

### Parameters


`data` - None

20-byte account address.

`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionCount",
"params": ["0xc94770007dda54cF92009BFF0dE90c06F603a09f", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x219"
}
```

