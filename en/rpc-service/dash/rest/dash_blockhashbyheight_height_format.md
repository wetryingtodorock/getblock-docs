---
title: dash:/blockhashbyheight/{height}{format} - Dash
description: Example code for the dash:/blockhashbyheight/{height}{format} rest method. Сomplete guide on how to use dash:/blockhashbyheight/{height}{format} rest in GetBlock.io Web3 documentation.
---

### Parameters


`height` - path

number, integer, required exactly 1

The height of the block hash to get

`format` - path

required, exactly 1

Set to .json for decoded block contents in JSON, or .bin or hex for a
serialized block in binary or hex

### Request

``` java
curl --location --request GET 'https://dash.getblock.io/mainnet/blockhashbyheight/1890110.json' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "blockhash": "000000000000000f190a64a90e753e02aed731731c863c47b5a1e3e3a3baf44c"
}
```

