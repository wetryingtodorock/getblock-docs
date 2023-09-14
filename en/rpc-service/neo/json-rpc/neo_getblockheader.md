---
title: neo:getblockheader \[POST\]
description: Returns the corresponding block header information according to thespecified script hash or index.The usage of this method is as same as getblock . The only difference isthat getblockeader gets the block header and getblock gets the completeblock.
---

### Parameters


`hash | index` - string or numeric

The block script hash or index (i.e. block height=number of blocks - 1).

`verbose` - bool or numeric, optional, default=false

When verbose is false, serialized information of the block is returned
in a hexadecimal string. If you need the detailed information, use the
SDK for deserialization.

When verbose is true or 1, detailed information of the block is returned
in Json format.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblockheader",
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
        "size": 676,
        "time": 1630403665,
        "version": 0
    }
}
```

