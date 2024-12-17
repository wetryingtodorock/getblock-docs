---
title: eth_feeHistory - Binance Smart Chain
description: Example code for the eth_feeHistory ws method. Сomplete guide on how to use eth_feeHistory ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA, 8 Bytes` - None

Number of blocks in the requested range.

`DATA, 32 Bytes` - None

Number of newest block in the requested range.

`DATA, 32 Bytes` - None

Optional monotonically increasing list of percentile values to sample
from each block's effective priority fees per gas in ascending order,
weighted by gas used.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_feeHistory",
"params": [61, "latest", [20, 60, 73]],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "baseFeePerGas": [
            "0x0",
            "0x0"
        ],
        "gasUsedRatio": [
            0.06900932857142857
        ],
        "oldestBlock": "0x1b5a241",
        "reward": [
            [
                "0xb2d05e00",
                "0xb2d05e00",
                "0xbebc2000"
            ]
        ]
    }
}
```

