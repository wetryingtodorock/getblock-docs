---
title: neo:getblock \[POST\]
description: Returns the corresponding block information according to the specifiedhash or index.The usage of this method is as same as getblockheader . The onlydifference is that getblockeader gets the block header and getblock getsthe complete block.
---

### Parameters


`hash |index` - string or numeric

Block hash string or block index (i.e. block height = number of blocks -
1).

`verbose` - bool or numeric, optional, default=false

When verbose is false, serialized information of the block is returned
in a Base64-encoded string. If you need the detailed information, use
SDK for deserialization.

When verbose is true or 1, detailed information of the block is returned
in Json format.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblock",
"params": ["0x63bbad22361ce78ded22d0ea375dc18b9121761e102856866e671e610395f55a", true],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "confirmations": 5037,
        "hash": "0x63bbad22361ce78ded22d0ea375dc18b9121761e102856866e671e610395f55a",
        "index": 7901849,
        "merkleroot": "0x8e786a973723e9c91f21f880f227d9281a2e09d001093535bd78fe17e0522af3",
        "nextblockhash": "0x60c8b06600ca523149328adee0d15be5b1f667833ef429b6114c9d09aaebd7f2",
        "nextconsensus": "AWjvTDuUHQLReAKj5ppqsvRRNtu4GhWmbU",
        "nonce": "38beb0b211f0f150",
        "previousblockhash": "0x83dcc81ca0c221153378b022f1d0032d2a14023ea538bc1101a65dd5bc7d9999",
        "script": {
            "invocation": "40a4f2df69a81b954c58307e3416909742c5ae8c600a1dae1f6acba7d4d40399a965fe3a3ef80d9ab2dd0a8bb83c76a569c9e7b0b877cb33636108d8e5fec18ae140ecfb152ffe2df959a1784b0ec88d60209901df9ce4a7cf5af6daec47d37a5cf327545369f8321fdf2752307923abe0e76f902e90653aa6e8a9f57afa4240169b40390330ed574ee59615299dd5dbaafa382171226e67532e11b4b0aad6e5e51357d29907147b347f3a109a15ab0f068a5fd2afa281dc33e02e5f8adf7e651e88604037daece4d197a0789d8da81e86568147ba3bb406bafbabe12c806d0cd7acd578059daa87db572f737acec2850f53cfc4352093bdeffe3d1127b01c5f7361f0a5404b91635d7621d7391158d00e43662ee02d08e276bad2b8c2daf9787932124eb4408f538bbde0cc9ef8d67ff16e6724a913bbd8b50ffbf7b06638d566d92dd1d0",
            "verification": "5521024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d21025bdf3f181f53e9696227843950deb72dcd374ded17c057159513c3d0abe20b642103b209fd4f53a7170ea4444e0cb0a6bb6a53c2bd016926989cf85f9b0fba17a70c2103b8d9d5771d8f513aa0869b9cc8d50986403b78c6da36890638c3d46a5adce04a2103c346b984b5ad1a7b0ab019f1550fd783108f83a6ca5396b152c7aa302b87ed5b2102ca0e27697b9c248f6f16e085fd0061e26f44da85b58ee835c110caa5ec3ba5542102df48f60e8f3e01c48ff40b9b7f1310d7a8b2a193188befe1c2e3df740e89509357ae"
        },
        "size": 25764,
        "time": 1630403665,
        "tx": [
            {
                "attributes": [],
                "net_fee": "0",
                "nonce": 301003088,
                "scripts": [],
                "size": 70,
                "sys_fee": "0",
                "txid": "0x2b64b0823f61a6be1a9b9fe2767a1e06b12a563a5f1d994b9adbc2387a907144",
                "type": "MinerTransaction",
                "version": 0,
                "vin": [],
                "vout": [
                    {
                        "address": "ASKnF2FnVg7DM8ZeWG2Ka9vS3f2Yt2Uv8j",
                        "asset": "0x602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7",
                        "n": 0,
                        "value": "0.00000064"
                    }
                ]
            },
            {
                "attributes": [
                    {
                        "data": "bd6530a0753da2afd9add8c5677e0afc16212ec8",
                        "usage": "Script"
                    }
                ],
                "gas": "0",
                "net_fee": "0.0000001",
                "script": "4d000165ddd609040a7c19ebffa59608019e5fc59570548450fda5f03151cc47e58b11fcb3b680a07909181b91239144c6f668d632c19e61490415df3119d2b9b0d20674939a554a1ebf4c8b5738f32c6c60293be8f51423edb0b2afa0a06e5f365f6bbe1d1db12ca11db8737513091110e873d0ef97d1babde387e3e7a6aa7d50ec54f8cc340f4eaffd99ca3ca1aed9a6a19eb72d9e709f8db1013996cd44fa733b2288be1144dcd92420f2fd067d1c34ad3c4608f24fb27cb56a1b33d5b8e1b89f56017f251a955cc1de087d7da18633e504e991fef281eb700b09a628a8036c3f3a5eaf7c9c0f92a7e946134734fe14e3e74ed0cf50b9add5150f1911ee3419db9b75043852dd6414b6cb731f90cefebbd4f9cedd0cf56bd1e21967f4147ba002bc1dbc918d555f1d466acda1d540332e2814378b147c06a7737a6a712d7bdcfa0d5bc3ca4d5314b6cb731f90cefebbd4f9cedd0cf56bd1e21967f454c1052642a45303052642a4530314bd6530a0753da2afd9add8c5677e0afc16212ec855c11673776170546f6b656e496e466f72546f6b656e4f757467aa47e2a95cc9ea59700144dd9f38ab356286a25e",
                "scripts": [
                    {
                        "invocation": "40829f48bfc9e5587779d9c414be559c27992b45e735fe32119ddd12b0f9716ff949ebde154eea7aae2565d09afef90a08e5d44026f4127b8517624f6895d54e76",
                        "verification": "21021c5115068d92190de216f81d29ba5879fb1593a37f615e331372663289c87509ac"
                    }
                ],
                "size": 656,
                "sys_fee": "0",
                "txid": "0x03696f36fe18a2b5d038e55c38921bfca96b94658097481f162c80699c467924",
                "type": "InvocationTransaction",
                "version": 0,
                "vin": [
                    {
                        "txid": "0x3a35d5a279a88e4af418cc1da7ec77ea0e33a6f51fe8d30f27d7228e3542b373",
                        "vout": 0
                    }
                ],
                "vout": [
                    {
                        "address": "AZ3JaZ9myjiW98hwLvc3F4RQVvVX4Pm83M",
                        "asset": "0x602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7",
                        "n": 0,
                        "value": "0.03170618"
                    }
                ]
            },
            {
                "attributes": [
                    {
                        "data": "bd6530a0753da2afd9add8c5677e0afc16212ec8",
                        "usage": "Script"
                    }
                ],
                "gas": "0",
                "net_fee": "0.0000001",
                "script": "4d000165ddd609040a7c19ebffa59608019e5fc59570548450fda5f03151cc47e58b11fcb3b680a07909181b91239144c6f668d632c19e61490415df3119d2b9b0d20674939a554a1ebf4c8b5738f32c6c60293be8f51423edb0b2afa0a06e5f365f6bbe1d1db12ca11db8737513091110e873d0ef97d1babde387e3e7a6aa7d50ec54f8cc340f4eaffd99ca3ca1aed9a6a19eb72d9e709f8db1013996cd44fa733b2288be1144dcd92420f2fd067d1c34ad3c4608f24fb27cb56a1b33d5b8e1b89f56017f251a955cc1de087d7da18633e504e991fef281eb700b09a628a8036c3f3a5eaf7c9c0f92a7e946134734fe14e3e74ed0cf50b9add5150f1911ee3419db9b75043852dd6414b6cb731f90cefebbd4f9cedd0cf56bd1e21967f4143c45a5bf36577453799f3e9ae9bf5bd569f6a83614a7c292d7903918a9e973a9fbfeab1b0b1793a81a14b6cb731f90cefebbd4f9cedd0cf56bd1e21967f454c1052642a45303052642a4530314bd6530a0753da2afd9add8c5677e0afc16212ec855c11673776170546f6b656e496e466f72546f6b656e4f757467aa47e2a95cc9ea59700144dd9f38ab356286a25e",
                "scripts": [
                    {
                        "invocation": "40fb8ee470af8edd21300d722b9919d13610bb660d5cf71f4f62d674095427ad6973d4b27b73da6860bef38b61e8c8957bf98fb0b01b3a16a7d4750be31ad238ee",
                        "verification": "21021c5115068d92190de216f81d29ba5879fb1593a37f615e331372663289c87509ac"
                    }
                ],
                "size": 656,
                "sys_fee": "0",
                "txid": "0x070caf64788c9c7bb78f56fa7a514c35220ed12ff1c3c507e4f391b5a04b7bfc",
                "type": "InvocationTransaction",
                "version": 0,
                "vin": [
                    {
                        "txid": "0x0b7604fe964d682df767b36ef8e1a26966ac4c706bad0496ca9505fea702503b",
                        "vout": 0
                    }
                ],
                "vout": [
                    {
                        "address": "AZ3JaZ9myjiW98hwLvc3F4RQVvVX4Pm83M",
                        "asset": "0x602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7",
                        "n": 0,
                        "value": "0.03136838"
                    }
                ]
            }
        ],
        "version": 0
    }
}
```

