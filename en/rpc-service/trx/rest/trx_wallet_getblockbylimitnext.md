---
title: trx:/wallet/getblockbylimitnext \[POST\]
description: Returns the list of Block Objects included in the Block Height rangespecified.
---

### Parameters


`startNum` - int32

Starting block height, including this block.

`endNum` - int32

Ending block height, excluding that block.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getblockbylimitnext' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"startNum": 30864542, "endNum": 30864544}'
```

###  Response

``` java
{
    "block": [
        {
            "blockID": "0000000001d6f49ebf6a4ff33cc1c1607145c48dc701fbd7ce00f410131e14f8",
            "block_header": {
                "raw_data": {
                    "number": 30864542,
                    "parentHash": "0000000001d6f49d0479eee63b80207fb66d24c1b7d50e2c89e0fd492861f508",
                    "timestamp": 1623055917000,
                    "txTrieRoot": "3739bc2a844d642506e8faf39d4012320ec1cf87899e1744e02b8d7f9ed2da3f",
                    "version": 21,
                    "witness_address": "41f29f57614a6b201729473c837e1d2879e9f90b8e"
                },
                "witness_signature": "4772f264935c69f0defe528a1b2c3cec91cfeb27b929364e59f75350594ebcf077ec6861c6461ac9696e518d6412882265cbd9eb05d97e72e00fbb8d2841a74f01"
            },
            "transactions": [
                {
                    "raw_data": {
                        "contract": [
                            {
                                "parameter": {
                                    "type_url": "type.googleapis.com/protocol.TransferAssetContract",
                                    "value": {
                                        "amount": 468000,
                                        "asset_name": "31303034303833",
                                        "owner_address": "411e4dc6d85c7f7cfe9ed92663ad558a23d04f1470",
                                        "to_address": "4151521c48d859021ffca3e9ace6b5f6364c44f46c"
                                    }
                                },
                                "type": "TransferAssetContract"
                            }
                        ],
                        "data": "42495320697320746865206d617070696e6720746f6b656e206f662074726332302e20496e766573746f72732063616e2065786368616e676520666f72205452582061742062696c6c73737761702e636f6d2028e694b6e588b0424953e9a085e79baee7a9bae68a95e794a8e688b6efbc8ce58fafe4bba5e588b0e5ae98e7b6b220687474703a2f2f62696c6c73737761702e636f6d20e5858ce68f9b54525829",
                        "expiration": 1623055971000,
                        "ref_block_bytes": "f48a",
                        "ref_block_hash": "7dbe57680f375514",
                        "timestamp": 1623055914588
                    },
                    "raw_data_hex": "0a02f48a22087dbe57680f37551440b8e5b2ad9e2f52a10142495320697320746865206d617070696e6720746f6b656e206f662074726332302e20496e766573746f72732063616e2065786368616e676520666f72205452582061742062696c6c73737761702e636f6d2028e694b6e588b0424953e9a085e79baee7a9bae68a95e794a8e688b6efbc8ce58fafe4bba5e588b0e5ae98e7b6b220687474703a2f2f62696c6c73737761702e636f6d20e5858ce68f9b545258295a75080212710a32747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e5472616e736665724173736574436f6e7472616374123b0a07313030343038331215411e4dc6d85c7f7cfe9ed92663ad558a23d04f14701a154151521c48d859021ffca3e9ace6b5f6364c44f46c20a0c81c70dcacafad9e2f",
                    "ret": [
                        {
                            "contractRet": "SUCCESS"
                        }
                    ],
                    "signature": [
                        "83778f8d27fd83ace18605747d1c3dd5606acf607f83e614a677e8ee41e7a3e12ea6cabdfec94325e887201f10f53c3ba022cad3bd87bcb8d3ad55f648a7ae3a01"
                    ],
                    "txID": "1097be146079d55633bcc1d6ddabb696797140474182d1ac8eced4b6e9aed8f1"
                }
            ]
        }
    ]
}
```

