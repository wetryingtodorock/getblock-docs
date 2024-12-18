---
title: getgrantong - Ontology
description: Example code for the getgrantong json-rpc method. Сomplete guide on how to use getgrantong json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`address` - string

base58 address

### Request

``` java
curl --location --request POST 'https://ont.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getgrantong",
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

