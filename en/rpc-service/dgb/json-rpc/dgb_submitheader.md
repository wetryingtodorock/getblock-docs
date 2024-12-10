---
title: dgb:submitheader  {disallowed} - DigiByte
description: Example code for the dgb:submitheader  {disallowed} json-rpc method. Сomplete guide on how to use dgb:submitheader  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`hexdata` - string, required

The hex-encoded block header data

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "submitheader",
"params": [null],
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

