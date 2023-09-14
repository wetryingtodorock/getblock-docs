---
title: ont:getbalancev2 \[POST\]
description: Return the allowance from the from account to the to account, with ONTsdecimals being 9, a ONGs decimals being 18.
---

### Parameters


`address` - string

Base58 address

### Request

``` java
curl --location --request POST 'https://ont.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getbalancev2",
"params": ["Adj7W5Z2hTeKH7YwJsfMzLuwiD671mvJ6X"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "desc": "SUCCESS",
    "error": 0,
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "height": "16224577",
        "ong": "9380961617034000000000",
        "ont": "14540000000000"
    }
}
```

