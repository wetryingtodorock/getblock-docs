---
title: neo:getcommittee \[POST\]
description: Gets the public key list of current Neo committee members.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getcommittee",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        "020f2887f41474cfeb11fd262e982051c1541418137c02a0f4961af911045de639",
        "03204223f8c86b8cd5c89ef12e4f0dbb314172e9241e30c9ef2293790793537cf0",
        "0222038884bbd1d8ff109ed3bdef3542e768eef76c1247aea8bc8171f532928c30",
        "0226933336f1b75baa42d42b71d9091508b638046d19abd67f4e119bf64a7cfb4d",
        "023a36c72844610b4d34d1968662424011bf783ca9d984efa19a20babf5582f3fe",
        "03409f31f0d66bdc2f70a9730b66fe186658f84a8018204db01c106edc36553cd0",
        "02486fd15702c4490a26703112a5cc1d0923fd697a33406bd5a1c00e0013b09a70",
        "024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d",
        "02504acbc1f4b3bdad1d86d6e1a08603771db135a73e61c9d565ae06a1938cd2ad",
        "03708b860c1de5d87f5b151a12c2a99feebd2e8b315ee8e7cf8aa19692a9e18379"
    ]
}
```

