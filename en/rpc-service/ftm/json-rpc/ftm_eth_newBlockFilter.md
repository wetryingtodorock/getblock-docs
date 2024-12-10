---
title: ftm:eth_newBlockFilter - Fantom
description: Example code for the ftm:eth_newBlockFilter json-rpc method. Сomplete guide on how to use ftm:eth_newBlockFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newBlockFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x91ade735d8e534290b7f774fd0e00b40"
}
```

