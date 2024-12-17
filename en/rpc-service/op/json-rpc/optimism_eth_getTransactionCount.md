---
title: optimism:eth_getTransactionCount \[POST\]
description: Returns the number of transactions sent from an address.
---

### Parameters


`DATA` - string

address.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionCount",
"params": ["0xbec4e80531dad6a9989828d174cc2878b1e3123d", "earliest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0"
}
```

