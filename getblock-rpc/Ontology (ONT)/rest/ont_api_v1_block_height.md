---
title: /api/v1/block/height - Ontology
description: Example code for the /api/v1/block/height rest method. Сomplete guide on how to use /api/v1/block/height rest in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/block/details/hash/d68a50c85d2ebe3e9c7b1613af3d588c65a64c1fa3043e58d4c6b70b51f5490e' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getblockbyhash",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": {
        "Hash": "d68a50c85d2ebe3e9c7b1613af3d588c65a64c1fa3043e58d4c6b70b51f5490e",
        "Header": {
            "BlockRoot": "f6fdb31745bf39331333daa4e71a9d65c8990df8e634bc648dfa33b949ae0199",
            "Bookkeepers": [
                "022bf80145bd448d993abffa237f4cd06d9df13eaad37afce5cb71d80c47b03feb",
                "035ab8d7b4a76a7c1d4efd7a204a26d6cf7afa3f2be23a9c55acd3f5c58e839248",
                "0251f06bc247b1da94ec7d9fe25f5f913cedaecba8524140353b826cf9b1cbd9f4"
            ],
            "ConsensusData": 9192128514454340632,
            "ConsensusPayload": "7b226c6561646572223a31302c227672665f76616c7565223a22424d524d4a395056517356783242677a412f55437a384243546b41352b437a3359424b6f6654785657474b4758376777794e752b526166717537794c355159336a394f6973536765306f557a53713754376b387977526b3d222c227672665f70726f6f66223a222f47763435794653494c2f38694462306a46476171335648384d786f6657515a68566749512b357747694b5951775062486f556f41786c6d4c6d34344e5369795a6172486f3235656b6758335337584456764c6257773d3d222c226c6173745f636f6e6669675f626c6f636b5f6e756d223a31363139343330302c226e65775f636861696e5f636f6e666967223a6e756c6c7d",
            "Hash": "d68a50c85d2ebe3e9c7b1613af3d588c65a64c1fa3043e58d4c6b70b51f5490e",
            "Height": 16242872,
            "NextBookkeeper": "AFmseVrdL9f9oyCzZefL9tG6UbvhPbdYzM",
            "PrevBlockHash": "0ca926e5b0d1a5fddf71f75b4a8f7eacc128f7c049254bc73a3b712385e3a7c0",
            "SigData": [
                "0c6c0225348c4a7b9fe9414bd2a19fcc4ea4f8cf14ec38d3b8ccfa125b4c08be01a12cb04f7235fa66aada869b747221e88f8cf2a876f5829f9f3ebd9f1b5b5d",
                "3a1364b7a3c3912e5a822d823169c529c9d74be3b7a47419fafee6c27a41f2d45ecc00e2f7a3bd7a6371115a08113350b53d5d50e693ff607a02e1556b9cc784",
                "4d2f9c7dc62b8ee3a193a4532eefdafde884d8fa55b4c42064c1aa733f423b93560244b67c1790d255b078021a212f8ab91f651635b531de8af448e488d1c6b7",
                "2a3bfd11e9db8d3baf0d67e306852bd3f8ed45ce12cafff560b97434430423def50ed0fafb03e20cb7bb23b6e7be5ef91e3fe8d1c306575d3d4589f5f4dafcd5"
            ],
            "Timestamp": 1687184058,
            "TransactionsRoot": "fb8660eee2cd98a8683daf4e06e0180b470896d68f6b8a4e4dffb1f18f68ff49",
            "Version": 0
        },
        "Size": 2195,
        "Transactions": [
            {
                "Attributes": [],
                "GasLimit": 3924288,
                "GasPrice": 3500,
                "Hash": "fb8660eee2cd98a8683daf4e06e0180b470896d68f6b8a4e4dffb1f18f68ff49",
                "Height": 16242872,
                "Nonce": 3698432840,
                "Payer": "AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW",
                "Payload": {
                    "Code": "057eafe1e21414e75e06f58cf3868f94a036c8622448806bd9a0da144565cd4515630e0f8a3e2d8241be2ec21e8e159553c1057eafe1e214144565cd4515630e0f8a3e2d8241be2ec21e8e15951464a222d3108f3dd8a896b7a73e71b40c1e75f11353c152c10d7472616e736665724d756c7469676d03a16843e61e5d96d389e178717ed57f9da4e5"
                },
                "Sigs": [
                    {
                        "M": 1,
                        "PubKeys": [
                            "024cde2ecca644ed84257251d7a31b37f3cbe19ab5b926f1ce2180e756d2f8a7a7"
                        ],
                        "SigData": [
                            "01ce6049a61eadd1dce57c3a765f5ddb101b50ee21cd2bc950ce03d3b77d2623d47cca3d1b3702cded9149f52b11de50c72ba7d74afa419c5b1557b47fa3f12309"
                        ]
                    },
                    {
                        "M": 1,
                        "PubKeys": [
                            "032db262ce294bf3889241995cb4682014e1b2ab89b3a1a8f3353b038c3a60b401"
                        ],
                        "SigData": [
                            "019a551a49214d4c6599b4d32fa6a412198e48b745e064d0bdb993a7dfae4b0f523c3685c61353de5deffa275c044fa83a94068cffa6eda1c8ebb0f43c0b361245"
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

