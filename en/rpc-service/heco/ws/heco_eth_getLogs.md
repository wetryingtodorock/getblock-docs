---
title: heco:eth_getLogs - Huobi ECO Chain
description: Example code for the heco:eth_getLogs ws method. Сomplete guide on how to use heco:eth_getLogs ws in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - object

The filter options

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getLogs",
"params": [{"topics": []}],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        {
            "address": "0xa71edc38d189767582c38a3145b5873052c3e47a",
            "blockHash": "0x250810cda6b7744f93c3eca5151a0e78937ef89c37a04513911785aa46d5aee3",
            "blockNumber": "0x18fd7b6",
            "data": "0x000000000000000000000000000000000000000000000010c966863f2c55a5a0",
            "logIndex": "0x0",
            "removed": false,
            "topics": [
                "0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef",
                "0x000000000000000000000000c14ee614bb53ef2405e5e52751cbdbe8ce76136f",
                "0x000000000000000000000000499b6e03749b4baf95f9e70eed5355b138ea6c31"
            ],
            "transactionHash": "0x9c9f22d8f8728a780aab284173fad7c6b5b462712df892013efd5b627192eeff",
            "transactionIndex": "0x0"
        },
        {
            "address": "0xa71edc38d189767582c38a3145b5873052c3e47a",
            "blockHash": "0x250810cda6b7744f93c3eca5151a0e78937ef89c37a04513911785aa46d5aee3",
            "blockNumber": "0x18fd7b6",
            "data": "0xfffffffffffffffffffffffffffffffffffffffffffb0985ec254765533f709f",
            "logIndex": "0x1",
            "removed": false,
            "topics": [
                "0x8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b925",
                "0x000000000000000000000000c14ee614bb53ef2405e5e52751cbdbe8ce76136f",
                "0x000000000000000000000000ed7d5f38c79115ca12fe6c0041abb22f0a06c300"
            ],
            "transactionHash": "0x9c9f22d8f8728a780aab284173fad7c6b5b462712df892013efd5b627192eeff",
            "transactionIndex": "0x0"
        },
        {
            "address": "0x5545153ccfca01fbd7dd11c0b23ba694d9509a6f",
            "blockHash": "0x250810cda6b7744f93c3eca5151a0e78937ef89c37a04513911785aa46d5aee3",
            "blockNumber": "0x18fd7b6",
            "data": "0x0000000000000000000000000000000000000000000000056c137a637e499951",
            "logIndex": "0x2",
            "removed": false,
            "topics": [
                "0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef",
                "0x000000000000000000000000499b6e03749b4baf95f9e70eed5355b138ea6c31",
                "0x000000000000000000000000c14ee614bb53ef2405e5e52751cbdbe8ce76136f"
            ],
            "transactionHash": "0x9c9f22d8f8728a780aab284173fad7c6b5b462712df892013efd5b627192eeff",
            "transactionIndex": "0x0"
        },
        {
            "address": "0x499b6e03749b4baf95f9e70eed5355b138ea6c31",
            "blockHash": "0x250810cda6b7744f93c3eca5151a0e78937ef89c37a04513911785aa46d5aee3",
            "blockNumber": "0x18fd7b6",
            "data": "0x0000000000000000000000000000000000000000000022255ee83847ec044ad70000000000000000000000000000000000000000000069765bea6fc8740b641d",
            "logIndex": "0x3",
            "removed": false,
            "topics": [
                "0x1c411e9a96e071241c2f21f7726b17ae89e3cab4c78be50e062b03a9fffbbad1"
            ],
            "transactionHash": "0x9c9f22d8f8728a780aab284173fad7c6b5b462712df892013efd5b627192eeff",
            "transactionIndex": "0x0"
        },
        {
            "address": "0x499b6e03749b4baf95f9e70eed5355b138ea6c31",
            "blockHash": "0x250810cda6b7744f93c3eca5151a0e78937ef89c37a04513911785aa46d5aee3",
            "blockNumber": "0x18fd7b6",
            "data": "0x0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010c966863f2c55a5a00000000000000000000000000000000000000000000000056c137a637e4999510000000000000000000000000000000000000000000000000000000000000000",
            "logIndex": "0x4",
            "removed": false,
            "topics": [
                "0xd78ad95fa46c994b6551d0da85fc275fe613ce37657fb8d5e3d130840159d822",
                "0x000000000000000000000000ed7d5f38c79115ca12fe6c0041abb22f0a06c300",
                "0x000000000000000000000000c14ee614bb53ef2405e5e52751cbdbe8ce76136f"
            ],
            "transactionHash": "0x9c9f22d8f8728a780aab284173fad7c6b5b462712df892013efd5b627192eeff",
            "transactionIndex": "0x0"
        }
    ]
}
```

