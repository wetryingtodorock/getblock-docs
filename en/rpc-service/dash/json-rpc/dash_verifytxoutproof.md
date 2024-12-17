---
title: dash:verifytxoutproof \[POST\]
description: Verifies that a proof points to one or more transactions in a block,returning the transactions the proof commits to and throwing an RPCerror if the block is not in our best block chain.
---

### Parameters


`proof` - string

A hex-encoded proof.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "verifytxoutproof",
"params": ["01000020ed72cc6a7294782a7711d8fa7ef74716ef062dc50bb0820f7eec923801000000aa5d17c5128043803b67c7ab03e4d3ffbc9604b54f877f1c5cf9ed3adeaa19b2cd7ed659f838011d10a70a480200000002033c89c2baecba9fc983c85dcf365c2d9cc93aca1dee2e5ac18124464056542e8faab0c579e651e9438c2904df5a498bc37a37acd528a251386fdef0476ba0e00105"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": [
        "e0a06b47f0de6f3851a228d5ac377ac38b495adf04298c43e951e679c5b0aa8f"
    ]
}
```

