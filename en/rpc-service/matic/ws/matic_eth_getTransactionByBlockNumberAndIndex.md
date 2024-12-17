---
title: eth_getTransactionByBlockNumberAndIndex - Polygon
description: Example code for the eth_getTransactionByBlockNumberAndIndex ws method. Сomplete guide on how to use eth_getTransactionByBlockNumberAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

`QUANTITY` - integer

Transaction index position.

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "accessList": [],
        "blockHash": "0x7cee929ba2e9522c0d5f4e80befc7543717ae2960168d334096b252a287a48ad",
        "blockNumber": "0x2958310",
        "chainId": "0x89",
        "from": "0x0a7832d7ec2a01b5b70fb9c84868202f8ea732d4",
        "gas": "0x30d40",
        "gasPrice": "0x833f4a34fc4",
        "hash": "0x294e21d7a8e420ad89d2605d6e12288ad52a2183756abf5a613672d7a8f0f0d7",
        "input": "0xbbc065c9000000000000000000000000000000000000000000000fedc19326dc970000000000000000000000000000000000000000000000000000000000000430e23400",
        "maxFeePerGas": "0x833f4a34fc4",
        "maxPriorityFeePerGas": "0x833f4a34fc4",
        "nonce": "0x90e3",
        "r": "0xee6094d6f347457025cdd86cccc024ca91ce00983009b0d1dbf6088514211982",
        "s": "0x769fdefa1bf9925e955ed933e737e462caee3ded5713cf1c9e899b44c1b6265c",
        "to": "0x26e57b5db7ae7aea946d960a871d93108ec0347b",
        "transactionIndex": "0x0",
        "type": "0x2",
        "v": "0x1",
        "value": "0x0"
    }
}
```

