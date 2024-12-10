---
title: dot:author_insertKey  {disallowed} - Polkadot
description: Example code for the dot:author_insertKey  {disallowed} json-rpc method. Сomplete guide on how to use dot:author_insertKey  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`keyType` - Text

key type

`suri` - Text

suri

`publicKey` - Bytes

public key

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "author_insertKey",
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

