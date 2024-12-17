---
title: ksm:mmr_verifyProofStateless \[POST\] {disallowed}
description: Verify an MMR proof statelessly given an mmr_root
---

### Parameters


`root` - MmmrHash

mmr hash

`proof` - MmmLeafBatchProof

mmr leaf batch proof

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "mmr_verifyProofStateless",
"params": [null, null],
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

