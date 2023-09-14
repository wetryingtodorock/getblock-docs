---
title: near:sandbox_patch_state \[POST\] {disallowed}
description: WARNING RPC endpoints in this section are only available on the localsandbox node.Patch account, access keys, contract code, or contract state. Onlyadditions and mutations are supported. No deletions. Account, accesskeys, contract code, and contract states have different formats. See theexample for details about their format.
---

### Parameters


`records` - array

an array of state records to patch. Every state record can be one of
Account, AccessKey, Contract (for contract code), or Data (for contract
state).

### Request

``` java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "sandbox_patch_state",
"params": [null],
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

