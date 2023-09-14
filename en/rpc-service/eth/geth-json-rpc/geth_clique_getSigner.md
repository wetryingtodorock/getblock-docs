---
title: geth:clique_getSigner \[POST\] {disallowed}
description: Returns the signer for a specific clique block. Can be called witheither a blocknumber, blockhash or an rlp encoded blob. The RLP encodedblob can either be a block or a header.
---

### Parameters


`block` - string

Block number, block Hash or encoded blob.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "clique_getSigner",
"params": ["0xfbaa33ae8b5a12bce04320f9fd609e30a300331c"],
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

