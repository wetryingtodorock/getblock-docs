---
title: dash:gettxoutsetinfo \[POST\]
description: Returns statistics about the confirmed unspent transaction output (UTXO)set. Note that this call may take some time and that it only countsoutputs from confirmed transactions - it does not count outputs from thememory pool.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "gettxoutsetinfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "bestblock": "0000000000000019cd3a50eedc418372f7aa9060d6ded56a769a51a93dfe0e4a",
        "bogosize": 324788089,
        "disk_size": 234663273,
        "hash_serialized_2": "01b22ab16971d4649f585441607dfc4d9ea9dd46e67e5264eb964b99e937b672",
        "height": 1535914,
        "total_amount": 10323909.43257612,
        "transactions": 1549909,
        "txouts": 4318861
    }
}
```

