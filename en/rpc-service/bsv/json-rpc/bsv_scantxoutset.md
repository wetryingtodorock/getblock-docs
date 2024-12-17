---
title: bsv:scantxoutset  {disallowed} - Bitcoin SV
description: Example code for the bsv:scantxoutset  {disallowed} json-rpc method. Сomplete guide on how to use bsv:scantxoutset  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`action` - string, required

The action to execute "start" for starting a scan "abort" for aborting
the current scan (returns true when abort was successful)

`scanobjects` - json array

Array of scan objects. Required for "start" action. Every scan object is
either a string descriptor or an object

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "scantxoutset",
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

