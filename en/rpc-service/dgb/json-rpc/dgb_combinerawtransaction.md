---
title: dgb:combinerawtransaction \[POST\]
description: Combine multiple partially signed transactions into one transaction.The combined transaction may be another partially signed transaction ora fully signed transaction.
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

