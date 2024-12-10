---
title: ont:gettransaction - Ontology
description: Example code for the ont:gettransaction ws method. Сomplete guide on how to use ont:gettransaction ws in GetBlock.io Web3 documentation.
---

### Parameters


`Raw` - string

When the value of the raw field in the request is set to 1, the API
returns serialized transaction information in the form of a hex string.
For 0, it returns raw information in the form of a JSON string. The
default value is 0.

`Hash` - string

transaction hash

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'gettransaction', 'Version': '1.0.0', 'Id': 1, 'Raw': '0', 'Hash': '3cda442a7798762de71cdbff64d6e7b8728aa5dbfa74670e1bb6ee2f0d89fdb9'}
```

###  Response

``` java
{
    "Action": "gettransaction",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "Attributes": [],
        "GasLimit": 3924288,
        "GasPrice": 2500,
        "Hash": "3cda442a7798762de71cdbff64d6e7b8728aa5dbfa74670e1bb6ee2f0d89fdb9",
        "Height": 16241692,
        "Nonce": 2716521183,
        "Payer": "AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW",
        "Payload": {
            "Code": "056f0c9e3b13144756eba570c7c9778418a0087be9c86a45487ac014c5f492260bbe04a7586dc4a70081a3440f0116c953c1056f0c9e3b1314c5f492260bbe04a7586dc4a70081a3440f0116c91464a222d3108f3dd8a896b7a73e71b40c1e75f11353c152c10d7472616e736665724d756c7469676d03a16843e61e5d96d389e178717ed57f9da4e5"
        },
        "Sigs": [
            {
                "M": 1,
                "PubKeys": [
                    "032046c26b5c8e89bfaf82f92b9220b430e78c7d2198f835efe72cc7cf7bc03502"
                ],
                "SigData": [
                    "010f0e8c89237d433e7f38308f2d59ae9acbce16be79f5bae9906cc2e77ee85c1730345f26b8be7759f41ca5f312f1974a13187853708915a20cb12a442487066e"
                ]
            },
            {
                "M": 1,
                "PubKeys": [
                    "032db262ce294bf3889241995cb4682014e1b2ab89b3a1a8f3353b038c3a60b401"
                ],
                "SigData": [
                    "01aec94d62f8405d14e0826950c4f653426929a5b5c6807e5862406823a8d6085e6d2d0467a51c99c492823b25e92abcea9f6723d6b73fb75d2aa0c100d25a5956"
                ]
            }
        ],
        "TxType": 209,
        "Version": 0
    },
    "Version": "1.0.0"
}
```

