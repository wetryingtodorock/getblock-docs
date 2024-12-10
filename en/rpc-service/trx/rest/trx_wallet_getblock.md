---
title: trx:/wallet/getblock - TRON
description: Example code for the trx:/wallet/getblock rest method. Сomplete guide on how to use trx:/wallet/getblock rest in GetBlock.io Web3 documentation.
---

### Parameters


`id_or_num` - string

id_or_num can be the block height or the block hash. No value entered
means to query the latest block.

`detail` - boolean

true means query the entire block information include the header and
body. false means only query the block header information.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getblock' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"id_or_num": "30864544", "detail": true}'
```

###  Response

``` java
{
    "blockID": "0000000001d6f4a09f60c27befccff6fe3cc593b2d6c46cdc79d3fd4f55db859",
    "block_header": {
        "raw_data": {
            "number": 30864544,
            "parentHash": "0000000001d6f49f615231bdeeddd8b563c746188d5e270a58afc87b059f29de",
            "timestamp": 1623055923000,
            "txTrieRoot": "cc12586dc14ca32175ff230931dfad4e2f57b71850948edae7ef1c7a7de08881",
            "version": 21,
            "witness_address": "41c81107148e5fa4b4a2edf3d5354db6c6be5b5549"
        },
        "witness_signature": "766ac978829f9c7d280e5de624162b12a8405e6e69b3955a2eac352c01ba48e20c7bcc31fa97f124a07fa68019ebcb3a93ee2f48493c5586a54bfaf978f786a601"
    },
    "transactions": [
        {
            "raw_data": {
                "contract": [
                    {
                        "parameter": {
                            "type_url": "type.googleapis.com/protocol.TransferContract",
                            "value": {
                                "amount": 50000000,
                                "owner_address": "41c33eeefda1059afba41d86759e281bcb851edfc8",
                                "to_address": "4158c85b7b6a5118beb3b23c14fcb2f3551a81d79a"
                            }
                        },
                        "type": "TransferContract"
                    }
                ],
                "expiration": 1623055977000,
                "ref_block_bytes": "f49e",
                "ref_block_hash": "bf6a4ff33cc1c160",
                "timestamp": 1623055920560
            },
            "raw_data_hex": "0a02f49e2208bf6a4ff33cc1c16040a894b3ad9e2f5a68080112640a2d747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e5472616e73666572436f6e747261637412330a1541c33eeefda1059afba41d86759e281bcb851edfc812154158c85b7b6a5118beb3b23c14fcb2f3551a81d79a1880e1eb1770b0dbafad9e2f",
            "ret": [
                {
                    "contractRet": "SUCCESS"
                }
            ],
            "signature": [
                "973e1cef0b8b2eb64e2ebe8a4ce69d9cce3c201a6b3885e853528f81383d19a67d35edd8e7027dba8e2f3211387fdef597e3f062a02a4d8aef990aaf2c29714d00"
            ],
            "txID": "979e0823f455f3b67d65b351052f0265233f422792d31d5dbeb7c24737dd5556"
        }
    ]
}
```

