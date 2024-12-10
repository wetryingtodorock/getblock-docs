---
title: btg:setlabel  {disallowed} - Bitcoin Gold
description: Example code for the btg:setlabel  {disallowed} json-rpc method. Сomplete guide on how to use btg:setlabel  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`address` - string, required

The bitcoin address to be associated with a label.

`label` - string, required

The label to assign to the address.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "setlabel",
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

