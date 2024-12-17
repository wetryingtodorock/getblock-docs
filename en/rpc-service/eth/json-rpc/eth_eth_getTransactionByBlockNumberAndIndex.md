---
title: eth:eth_getTransactionByBlockNumberAndIndex - Ethereum
description: Example code for the eth:eth_getTransactionByBlockNumberAndIndex json-rpc method. Сomplete guide on how to use eth:eth_getTransactionByBlockNumberAndIndex json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

`QUANTITY` - None

The transaction index position.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionByBlockNumberAndIndex",
"params": ["0x52A96E", "0x1"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "blockHash": "0x7f0c47c49d70010028085c26f2fa9dfd7b6406a86fd522610f70852249632a81",
        "blockNumber": "0x52a96e",
        "chainId": "0x1",
        "from": "0xfbb1b73c4f0bda4f67dca266ce6ef42f520fbb98",
        "gas": "0x249f0",
        "gasPrice": "0xba43b7400",
        "hash": "0x0bf895891745037c4dce90f873b84cccd37396abcf32d113154b82fe16016b0d",
        "input": "0xa9059cbb0000000000000000000000009f050bc566289fe08f9534eb8b5b7437071a85ca000000000000000000000000000000000000000000000589b9c8aed550c82400",
        "nonce": "0x515f4c",
        "r": "0xe0ec15e49c7ef372fe7393dbb814bc69a007a89632f2921a540a6b975a2099cf",
        "s": "0x62f9e1d600011370d83c8ec2a04f0d4e406eb286120c8c0767ff176b3ac1789d",
        "to": "0xa74476443119a942de498590fe1f2454d7d4ac0d",
        "transactionIndex": "0x1",
        "type": "0x0",
        "v": "0x26",
        "value": "0x0"
    }
}
```

