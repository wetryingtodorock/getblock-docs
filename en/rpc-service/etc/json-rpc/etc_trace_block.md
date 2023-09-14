---
title: etc:trace_block \[POST\]
description: Provides transaction processing of type trace for the specified block.
---

### Parameters


`quantity|tag` - string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "trace_block",
"params": ["latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        {
            "action": {
                "author": "0xdf7d7e053933b5cc24372f878c90e62dadad5d42",
                "rewardType": "block",
                "value": "0x2c68af0bb1400000"
            },
            "blockHash": "0xf71c2351b989bbec7e8172e3b97cd91516ddab6895021a7c94eed05cc00ff8a9",
            "blockNumber": 13522687,
            "result": null,
            "subtraces": 0,
            "traceAddress": [],
            "transactionHash": null,
            "transactionPosition": null,
            "type": "reward"
        }
    ]
}
```

