---
title: sendrawtransaction - Ontology
description: Example code for the sendrawtransaction ws method. Сomplete guide on how to use sendrawtransaction ws in GetBlock.io Web3 documentation.
---

### Parameters


`PreExec` - integer

The PreExec field in the request object is used to specify whether the
contract needs to be pre-run. If the contract is to be pre-run, set the
value to 1, else 0.

`Data` - string

raw transaction data

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'sendrawtransaction', 'Version': '1.0.0', 'Id': 1, 'Data': '00d1dfd2eaa1c40900000000000040e13b000000000064a222d3108f3dd8a896b7a73e71b40c1e75f11389056f0c9e3b13144756eba570c7c9778418a0087be9c86a45487ac014c5f492260bbe04a7586dc4a70081a3440f0116c953c1056f0c9e3b1314c5f492260bbe04a7586dc4a70081a3440f0116c91464a222d3108f3dd8a896b7a73e71b40c1e75f11353c152c10d7472616e736665724d756c7469676d03a16843e61e5d96d389e178717ed57f9da4e500024241010f0e8c89237d433e7f38308f2d59ae9acbce16be79f5bae9906cc2e77ee85c1730345f26b8be7759f41ca5f312f1974a13187853708915a20cb12a442487066e2321032046c26b5c8e89bfaf82f92b9220b430e78c7d2198f835efe72cc7cf7bc03502ac424101aec94d62f8405d14e0826950c4f653426929a5b5c6807e5862406823a8d6085e6d2d0467a51c99c492823b25e92abcea9f6723d6b73fb75d2aa0c100d25a59562321032db262ce294bf3889241995cb4682014e1b2ab89b3a1a8f3353b038c3a60b401ac'}
```

###  Response

``` java
{
    "Action": "sendrawtransaction",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": "22471ab3f4b4307a99f00c9a717dbf8b26f5bf63bf47f9c560477da8181de777",
    "Version": "1.0.0"
}
```

