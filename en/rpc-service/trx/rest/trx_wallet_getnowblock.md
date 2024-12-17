---
title: /wallet/getnowblock - TRON
description: Example code for the /wallet/getnowblock rest method. Сomplete guide on how to use /wallet/getnowblock rest in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getnowblock' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "blockID": "0000000002dbe0e890dddd5df8bb75251f386daee6e5b7a6cf777d493e5d894c",
    "block_header": {
        "raw_data": {
            "number": 47964392,
            "parentHash": "0000000002dbe0e7cfc367b39b54d4a53beda9b70a493a724561cad264f38e37",
            "timestamp": 1674492219000,
            "txTrieRoot": "3b9e119fe6a0807baa98fdb1e20e5100772e3173eb14f7be424a5e66ac99503a",
            "version": 26,
            "witness_address": "417f5e5aca5332ce5e18414d7f85bb62097cefa453"
        },
        "witness_signature": "1a12774cf941968707f2bff2f39352953211630399223631f5a7f3ca5dfd6bd126e9ff83a60a1d2e906229d492ee967f1359fb18bc58a291deedbda9e2ff7f7801"
    },
    "transactions": [
        {
            "raw_data": {
                "contract": [
                    {
                        "parameter": {
                            "type_url": "type.googleapis.com/protocol.TransferContract",
                            "value": {
                                "amount": 1,
                                "owner_address": "41a7b6965481021cc80e0d78a921b60a7b45fdbeb5",
                                "to_address": "4162d0adca402b12e898b8d3a2debc77ce41c8ecc4"
                            }
                        },
                        "type": "TransferContract"
                    }
                ],
                "expiration": 1674492273000,
                "ref_block_bytes": "e0d4",
                "ref_block_hash": "1394b476dff14ddd",
                "timestamp": 1674492216461
            },
            "raw_data_hex": "0a02e0d422081394b476dff14ddd40e8c291fcdd305a65080112610a2d747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e5472616e73666572436f6e747261637412300a1541a7b6965481021cc80e0d78a921b60a7b45fdbeb512154162d0adca402b12e898b8d3a2debc77ce41c8ecc41801708d898efcdd30",
            "ret": [
                {
                    "contractRet": "SUCCESS"
                }
            ],
            "signature": [
                "ccedee74d57ec4409d0e1b77f329716843790df0a1a2281c244c6d5e0d2e6fb7085b451da3d4cba1436c81825c9a6ef79fc5c846d428090203a484c5319fd0a400"
            ],
            "txID": "30232b8c605f7a3651390ac5fd69d2f8d244791624e9f03d190f5d6cb465bb5e"
        }
    ]
}
```

