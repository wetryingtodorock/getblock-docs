---
title: dgb:combinerawtransaction - DigiByte
description: Example code for the dgb:combinerawtransaction json-rpc method. Сomplete guide on how to use dgb:combinerawtransaction json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`txs` - json array, required

A json array of hex strings of partially signed transactions

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "combinerawtransaction",
"params": [["myhex1", "myhex2", "myhex3"]],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": null
}
```

