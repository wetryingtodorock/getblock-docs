---
title: bsc:eth_newPendingTransactionFilter - Binance Smart Chain
description: Example code for the bsc:eth_newPendingTransactionFilter json-rpc method. Сomplete guide on how to use bsc:eth_newPendingTransactionFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newPendingTransactionFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xe4e164bfaa484b9b998772b6dfe9c7cd"
}
```

