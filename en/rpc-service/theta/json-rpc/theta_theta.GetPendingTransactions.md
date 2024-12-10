---
title: theta:theta.GetPendingTransactions - Theta Network
description: Example code for the theta:theta.GetPendingTransactions json-rpc method. Сomplete guide on how to use theta:theta.GetPendingTransactions json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://theta.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "theta.GetPendingTransactions",
"params": {},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "tx_hashes": [
            "0x61ed06b78fededbbd262f95f321d7e48dee81e9b1e493b7f4d42c6bf7afd4b27",
            "0xc4162541f5e9f283bd9c3beb2798a4a2539b567dd35f52edefde7063f985ab17"
        ]
    }
}
```

