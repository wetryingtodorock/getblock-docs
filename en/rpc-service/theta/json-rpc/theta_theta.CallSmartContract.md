---
title: theta:theta.CallSmartContract - Theta Network
description: Example code for the theta:theta.CallSmartContract json-rpc method. Сomplete guide on how to use theta:theta.CallSmartContract json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`sctx_bytes` - string

the signed transaction bytes.

### Request

``` java
curl --location --request POST 'https://theta.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "theta.CallSmartContract",
"params": {"sctx_bytes": "02f8a4c78085e8d4a51000f86ff86d942e833968e5bb786ae419c4d13189fb081cc43babd3888ac7230489e800008901158e46f1e875100016b841393e2eba6241482098cf11ef4dd869209d7ebd716397f3c862ca5b762bbf403006b1fa009786102383c408cabdf7450c1c73d4dd4a20d3b48a39a88ffe0ecb0e01eae9949f1233798e905e173560071255140b4a8abd3ec6d3888ac7230489e800008901158e460913d00000"},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

