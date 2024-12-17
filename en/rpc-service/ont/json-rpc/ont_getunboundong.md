---
title: ont:getunboundong \[POST\]
description: Fetch the amount of unbound ONG that can be withdrawn for a particularaddress.
---

### Parameters


`address` - string

address

### Request

``` java
curl --location --request POST 'https://ont.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getunboundong",
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
    "result": "0"
}
```

