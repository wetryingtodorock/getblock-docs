---
title: dash:decodescript \[POST\]
description: Decodes a hex-encoded P2SH redeem script.
---

### Parameters


`Redeem Script` - string (hex)

The redeem script to decode as a hex-encoded serialized script.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "decodescript",
"params": ["76a9147c086eada12bdb10a265c16c08a7ae87366bd48188ac"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "addresses": [
            "XmzfivrzYQ7B7oBMZKwPRdhjB1iNvX71XZ"
        ],
        "asm": "OP_DUP OP_HASH160 7c086eada12bdb10a265c16c08a7ae87366bd481 OP_EQUALVERIFY OP_CHECKSIG",
        "p2sh": "7n9YufoWBrJ65YC7sgwk53EzbPHMQRB6HJ",
        "reqSigs": 1,
        "type": "pubkeyhash"
    }
}
```

