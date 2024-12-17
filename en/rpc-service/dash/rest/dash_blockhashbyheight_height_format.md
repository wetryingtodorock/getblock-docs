---
title: dash:/blockhashbyheight/{height}{format} \[GET\]
description: The GET blockhashbyheight operation returns the hash of a block inbest-block-chain at the height provided. The hash can be returned as aJSON object or serialized as binary or hex.
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

