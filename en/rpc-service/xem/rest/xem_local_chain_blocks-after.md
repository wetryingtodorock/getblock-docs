---
title: xem:/local/chain/blocks-after \[POST\] {disallowed}
description: Gets up to 10 blocks after given block height from the chain. If thedatabase contains less than 10 block after the given height, then lessblocks are returned.
---

### Parameters


`height` -

A BlockHeight JSON object. The block height describes the position of
the block within the block chain. The first block of the chain has
height one. Each subsequent block has a height which is one higher than
the previous block. The following structure is used by the NEM block
chain explorer for convenience reason.

### Request

``` java
curl --location --request POST 'https://xem.getblock.io/local/chain/blocks-after'
 --header 'x-api-key: YOUR-API-KEY'
 --header 'Content-Type: application/json'
 --data-raw '{'height':3943115}'
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

