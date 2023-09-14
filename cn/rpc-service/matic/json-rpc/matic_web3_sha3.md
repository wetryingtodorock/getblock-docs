---
title: matic:web3_sha3 \[POST\]
description: Returns Keccak-256 (not the standardized SHA3-256) of the given data.
---

### Parameters


`DATA` - array of string

the data to convert into a SHA3 hash.

### Request

``` java
curl --location --request POST 'https://matic.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "web3_sha3",
"params": ["0xf2a2b854721d4372474fc76cc13445a73369c0c334f4935c88bde3c310f28c9a"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xf5d3389b32cee33308ce9af2d8aefa1517aa90ccb7b1d2eb29c61f13e1fd3cea"
}
```

