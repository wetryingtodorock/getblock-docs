---
title: rsk:eth_getLogs \[POST\]
description: Returns an array of all logs matching a given filter object.
---

### Parameters


`Object` - object

The filter options

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
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
            "address": "0x461750b4824b14c3d9b7702bc6fbb82469082b23",
            "blockHash": "0xce6eaa95170f1d59d5bd971a4a8e3de38e795a063fb1ebcfa3e9d5a6af1635a3",
            "blockNumber": "0x526f5f",
            "data": "0x0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000000000000000000000645a6866990000000000000000000000000000000000000000000000000134227e9baf1c4900000000000000000000000000000000000000000000000000000000649078f8000000000000000000000000504efcadfb020d6bbaec8a5c5bb21453719d0e00",
            "logIndex": "0x0",
            "topics": [
                "0x5a68669900000000000000000000000000000000000000000000000000000000",
                "0x000000000000000000000000d554a563adfd9198782add9ad7554c6ffe87ef09",
                "0x0000000000000000000000000000000000000000000000000134227e9baf1c49",
                "0x00000000000000000000000000000000000000000000000000000000649078f8"
            ],
            "transactionHash": "0xbbf9233fc0040143409d9cfdc81243359f4c7488d71aa678d6f262f11be4c6aa",
            "transactionIndex": "0x0"
        },
        {
            "address": "0x504efcadfb020d6bbaec8a5c5bb21453719d0e00",
            "blockHash": "0xce6eaa95170f1d59d5bd971a4a8e3de38e795a063fb1ebcfa3e9d5a6af1635a3",
            "blockNumber": "0x526f5f",
            "data": "0x0000000000000000000000000000000000000000000000000134216039f82e25",
            "logIndex": "0x1",
            "topics": [
                "0x296ba4ca62c6c21c95e828080cb8aec7481b71390585605300a8a76f9e95b527"
            ],
            "transactionHash": "0xbbf9233fc0040143409d9cfdc81243359f4c7488d71aa678d6f262f11be4c6aa",
            "transactionIndex": "0x0"
        },
        {
            "address": "0x7ecfda6072942577d36f939ad528b366b020004b",
            "blockHash": "0xce6eaa95170f1d59d5bd971a4a8e3de38e795a063fb1ebcfa3e9d5a6af1635a3",
            "blockNumber": "0x526f5f",
            "data": "0x0000000000000000000000000000000000000000000000000000000000526f5d00000000000000000000000000000000000000000000000000000000010b40f600000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000e000000000000000000000000000000000000000000000000000000000000001400000000000000000000000000000000000000000000000000000000000000005322e302e31000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002652736b4a2f342e322e302f4c696e75782f4a617661312e382f484f502d65616638653539303800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000031476574682f76312e31312e352d737461626c652d61333866343130382f6c696e75782d616d6436342f676f312e32302e32000000000000000000000000000000",
            "logIndex": "0x0",
            "topics": [
                "0xbb00e6cbdccbb5b7549e189335249187223d88583604555326aa1d7ccbcad442",
                "0x000000000000000000000000a4398c6ff62e9b93b32b28dd29bd27c6b106245f"
            ],
            "transactionHash": "0xa0b6086ed57d3e3ffbadaadf3813288b991466dcbdbc7b80964666026f54110f",
            "transactionIndex": "0x1"
        }
    ]
}
```
