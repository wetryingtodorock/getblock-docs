---
title: eth_newPendingTransactionFilter - Fantom
description: Example code for the eth_newPendingTransactionFilter json-rpc method. Сomplete guide on how to use eth_newPendingTransactionFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
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
    "result": "0xc2fb10e567fe5ed6d92e5cdca4bee7da"
}
```
