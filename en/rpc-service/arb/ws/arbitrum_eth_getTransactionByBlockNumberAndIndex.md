---
title: arbitrum:eth_getTransactionByBlockNumberAndIndex \[WebSocket\]
description: Returns information about a transaction by block number and transactionindex position.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

`QUANTITY` - integer

Transaction index position.

### Request

``` java
wscat -c wss://arbitrum.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getTransactionByBlockNumberAndIndex",
"params": ["latest", "0x0"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "blockHash": "0x92ab138d1693f96884d613d2ecd8cd13307a4eeccabec9dd9d6ce2b0e0aae62e",
        "blockNumber": "0x5bc416f",
        "chainId": "0xa4b1",
        "from": "0x00000000000000000000000000000000000a4b05",
        "gas": "0x0",
        "gasPrice": "0x0",
        "hash": "0xbf837afe75a55d743fe901088126e90d8762756b83ebe9f03e0a568b6fd45918",
        "input": "0x6bf6a42d000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010924a90000000000000000000000000000000000000000000000000000000005bc416f0000000000000000000000000000000000000000000000000000000000000000",
        "nonce": "0x0",
        "r": "0x0",
        "s": "0x0",
        "to": "0x00000000000000000000000000000000000a4b05",
        "transactionIndex": "0x0",
        "type": "0x6a",
        "v": "0x0",
        "value": "0x0"
    }
}
```

