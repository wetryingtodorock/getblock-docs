---
title: xmr:relay_tx \[POST\]
description: Relay a list of transaction IDs.
---

### Parameters

`txids` - array of string

list of transaction IDs to relay

### Request

``` java
curl --location --request POST 'https://xmr.getblock.io/mainnet/json_rpc' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "relay_tx",
"params": {"txids": "9fd75c429cbe52da9a52f2ffc5fbd107fe7fd2099c0d8de274dc8a67e0c98613"},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "credits": 0,
        "status": "OK",
        "top_hash": "",
        "untrusted": false
    }
}
```
