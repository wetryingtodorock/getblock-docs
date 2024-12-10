---
title: btg:bumpfee  {disallowed} - Bitcoin Gold
description: Example code for the btg:bumpfee  {disallowed} json-rpc method. Сomplete guide on how to use btg:bumpfee  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`txid` - string, required

The txid to be bumped

`options` - json object, optional

The txid to be bumped

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "bumpfee",
"params": [null, null],
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

