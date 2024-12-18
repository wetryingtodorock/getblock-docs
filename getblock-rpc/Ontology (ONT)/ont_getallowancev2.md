---
title: getallowancev2  {disallowed} - Ontology
description: Example code for the getallowancev2  {disallowed} json-rpc method. Сomplete guide on how to use getallowancev2  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`ont` - string

ammount of allowance

`from` - string

from address

`to` - string

to address

### Request

``` java
curl --location --request POST 'https://ont.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getallowancev2",
"params": [null, null, null],
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

