---
title: dash:getmerkleblocks \[POST\]
description: Returns an array of hex-encoded merkleblocks for blocks starting fromwhich match.
---

### Parameters


`filter` - string

The hex encoded bloom filter.

`hash` - string

The block hash.

`count` - number (int)

Optional.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getmerkleblocks",
"params": ["2303028005802040100040000008008400048141010000f8400420800080025004000004130000000000000001", "00000000007e1432d2af52e8463278bf556b55cf5049262f25634557e2e91202", 2000],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": [
        "000000202c...aefc440107",
        "0000002058...9a17830103"
    ]
}
```

