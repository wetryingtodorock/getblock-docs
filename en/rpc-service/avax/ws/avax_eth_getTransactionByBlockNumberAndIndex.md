---
title: avax:eth_getTransactionByBlockNumberAndIndex - Avalanche
description: Example code for the avax:eth_getTransactionByBlockNumberAndIndex ws method. Сomplete guide on how to use avax:eth_getTransactionByBlockNumberAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

`QUANTITY` - string

Transaction index position.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "blockHash": "0x3fb8949661bb2f6f5eaa5b16318d3c7e7a0990f8c2382d1fe4389e0caac6519d",
        "blockNumber": "0x1d61350",
        "chainId": "0xa86a",
        "from": "0xdc32cac19d77ad8f6b64094dd39b2e441d997e03",
        "gas": "0x2dc6c0",
        "gasPrice": "0x95e560e93",
        "hash": "0x027c4627cf327e492f96c02e58d913530a7fd7436945b96fbe9a2c26fdee93ac",
        "input": "0x17835d1c00000000000000000000000000000000001cddd5019e6876019e687600003869000000000000000000000000000000000000000000000000000000006479b045",
        "maxFeePerGas": "0x48c27395000",
        "maxPriorityFeePerGas": "0x37e11d600",
        "nonce": "0xa472",
        "r": "0xa1ebd13006d631b98451bf9ea2fd6e86c9026a6f6d7cfee75d1bc270b35c0198",
        "s": "0x5ef1746f1a13d0a861f51bfeb6d6b2c24a97aeb92328771b1c5406d03f4b1fc8",
        "to": "0xe547cadbe081749e5b3dc53cb792dfaea2d02fd2",
        "transactionIndex": "0x0",
        "type": "0x2",
        "v": "0x1",
        "value": "0x0"
    }
}
```

