---
title: trx:/wallet/getblockbylatestnum \[POST\]
description: Returns a list of block objects.
---

### Parameters


`num` - int32

The number of blocks to query

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getblockbylatestnum' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"num": 2}'
```

###  Response

``` java
{
    "block": [
        {
            "blockID": "0000000002dbe0e7cfc367b39b54d4a53beda9b70a493a724561cad264f38e37",
            "block_header": {
                "raw_data": {
                    "number": 47964391,
                    "parentHash": "0000000002dbe0e63d1c2c9bfe2b506b60c627bb8b6923b89c0b52fdb05a680c",
                    "timestamp": 1674492216000,
                    "txTrieRoot": "a5bcc19964ae310d23713e9c7e5b7f8f18dce2cff43a1fa535138190cdc55e17",
                    "version": 26,
                    "witness_address": "41d376d829440505ea13c9d1c455317d51b62e4ab6"
                },
                "witness_signature": "766505fbdf732991963e592b7d80d1372ccc464653fbb47a0d80f15bc3e914e278a89bb7c3fbac33e7a5bbac893c555a432baad13b4ce3f9a1dd6175e2b70cf400"
            },
            "transactions": [
                {
                    "raw_data": {
                        "contract": [
                            {
                                "parameter": {
                                    "type_url": "type.googleapis.com/protocol.TransferContract",
                                    "value": {
                                        "amount": 20000000,
                                        "owner_address": "41b0e9c2f2cf6edf58521a1bae6b8b327b3c8d6197",
                                        "to_address": "4150569bb3f1905617429e712b4ceee97af0a0e7b9"
                                    }
                                },
                                "type": "TransferContract"
                            }
                        ],
                        "expiration": 1674492270000,
                        "ref_block_bytes": "e0d3",
                        "ref_block_hash": "6389d24629d1dacc",
                        "timestamp": 1674492212784
                    },
                    "raw_data_hex": "0a02e0d322086389d24629d1dacc40b0ab91fcdd305a68080112640a2d747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e5472616e73666572436f6e747261637412330a1541b0e9c2f2cf6edf58521a1bae6b8b327b3c8d619712154150569bb3f1905617429e712b4ceee97af0a0e7b91880dac40970b0ec8dfcdd30",
                    "ret": [
                        {
                            "contractRet": "SUCCESS"
                        }
                    ],
                    "signature": [
                        "54816a0e294c97039312f1e38003b2017206553b4bde6dcf98969349d010bbf0531f1dbae02240e468b55cb4af0faa53e38321d1b83317cf811d001f4a7ba6ca00"
                    ],
                    "txID": "59352daf0d6fa1d9ea4eb4c1eb6a6e664c7a1f3ffdbe51842eaa7e675b7ca1df"
                }
            ]
        }
    ]
}
```

