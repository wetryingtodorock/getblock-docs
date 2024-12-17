---
title: dgb:settxfee  {disallowed} - DigiByte
description: Example code for the dgb:settxfee  {disallowed} json-rpc method. Сomplete guide on how to use dgb:settxfee  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`amount` - numeric or string, required

The transaction fee in BTC/kvB

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "settxfee",
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

