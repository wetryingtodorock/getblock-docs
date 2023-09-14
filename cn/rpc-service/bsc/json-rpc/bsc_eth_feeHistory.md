---
title: bsc:eth_feeHistory \[POST\]
description: Returns a list of historical gas information.
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
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_feeHistory",
"params": [61, "latest", [20, 60, 73]],
"id": "getblock.io"}'
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
            0.10737980714285714
        ],
        "oldestBlock": "0x1b5a217",
        "reward": [
            [
                "0xb2d05e00",
                "0xb2d05e00",
                "0xb2d05e00"
            ]
        ]
    }
}
```

