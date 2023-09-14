---
title: ont:getblockbyhash \[WebSocket\]
description: Fetch block details for block using given block hash.
---

### Parameters


`Raw` - string

When the value of the raw field in the request is set to 1, the API
returns serialized block information in the form of a hex string. For 0,
it returns raw information in the form of a JSON string. The default
value is 0.

`Hash` - string

block hash

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getblockbyhash', 'Version': '1.0.0', 'Id': 1, 'Raw': '0', 'Hash': '810c6b7329e664dfdd21e4a642bec16e0c8982d0c7add37e5d16bf5527206d2a'}
```

###  Response

``` java
{
    "Action": "getblockbyhash",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "Hash": "810c6b7329e664dfdd21e4a642bec16e0c8982d0c7add37e5d16bf5527206d2a",
        "Header": {
            "BlockRoot": "dc30ab4e123c42d1d18006ab891e75ca253a2d4c5beed1fb549a90c058d6c03b",
            "Bookkeepers": [
                "022bf80145bd448d993abffa237f4cd06d9df13eaad37afce5cb71d80c47b03feb",
                "035ab8d7b4a76a7c1d4efd7a204a26d6cf7afa3f2be23a9c55acd3f5c58e839248",
                "02496da03a2108868cc3e443911438428e98029e481b26aaa140f796cd2abc4664"
            ],
            "ConsensusData": 15359481140379161185,
            "ConsensusPayload": "7b226c6561646572223a31302c227672665f76616c7565223a2242462f3262562f7449364f7a5065376e7165776958396b46783872422f6143494e727137324d524770544e3346536b61516d6a3855686b43546247782f454b6a7a63437064565a31384c3076764639545a677858554b733d222c227672665f70726f6f66223a225a6c4f5a4f6d2f68386e7663794b7433526a36314f3035323762785463712f785a476d4a796130616967582f5147316f78675a306264456368664e757737702f44796f4c424e6f3855634c506b41477a717a6a2b7a773d3d222c226c6173745f636f6e6669675f626c6f636b5f6e756d223a31363139343330302c226e65775f636861696e5f636f6e666967223a6e756c6c7d",
            "Hash": "810c6b7329e664dfdd21e4a642bec16e0c8982d0c7add37e5d16bf5527206d2a",
            "Height": 16241692,
            "NextBookkeeper": "AFmseVrdL9f9oyCzZefL9tG6UbvhPbdYzM",
            "PrevBlockHash": "81a493f165951f401af8552d36daa8c6220a786606dc00a2e5813009cae49e67",
            "SigData": [
                "4bce0c3363d85331f77abaad0c01a524649481cad2c4e10c621a06d26cec4140dee5c91bf7fa54158e4e3fd3f47c8b60f0a897f598bd5e730aa1d7961c2a3d0f",
                "44e7e7d73702417e1cf9576bf985fe0e55a043c1e5e5995472367227d27d8c011f93a7ffc7a5549627ebdf62c23a6f60ac4f7a44f71c165269829769128f9559",
                "2718d82a1551304bb04a7c294aafefd29046c0c4c82824a686a966ea581b05566465ddb9ed67b470fe6f19651841dfea04082e96aa75db8c1b72e61f2ea37543"
            ],
            "Timestamp": 1687168080,
            "TransactionsRoot": "3cda442a7798762de71cdbff64d6e7b8728aa5dbfa74670e1bb6ee2f0d89fdb9",
            "Version": 0
        },
        "Size": 2096,
        "Transactions": [
            {
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
            }
        ]
    },
    "Version": "1.0.0"
}
```

