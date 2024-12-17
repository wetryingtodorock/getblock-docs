---
title: dgb:fundrawtransaction \[POST\]
description: If the transaction has no inputs, they will be automatically selected tomeet its out value.It will add at most one change output to the outputs.No existing outputs will be modified unless subtractFeeFromOutputs isspecified.Note that inputs which were signed may need to be resigned aftercompletion since in/outputs have been added.The inputs added will not be signed, use signrawtransactionwithkey orsignrawtransactionwithwallet for that.Note that all existing inputs must have their previous outputtransaction be in the wallet.Note that all inputs selected must be of standard form and P2SH scriptsmust be in the wallet using importaddress or addmultisigaddress (tocalculate fees).You can see whether this is the case by checking the solvable field inthe listunspent output.Only pay-to-pubkey, multisig, and P2SH versions thereof are currentlysupported for watch-only.
---

### Parameters


`hexstring` - string, required

The hex string of the raw transaction

`options` - json object, optional

for backward compatibility: passing in a true instead of an object will
result in {"includeWatching":true}

`iswitness` - boolean, optional, default=depends on heuristic tests

Whether the transaction hex is a serialized witness transaction.

If iswitness is not present, heuristic tests will be used in decoding.

If true, only witness deserialization will be tried.

If false, only non-witness deserialization will be tried.

This boolean should reflect whether the transaction has inputs (e.g.
fully valid, or on-chain transactions), if known by the caller.

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "fundrawtransaction",
"params": ["010000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff580426efcf00042d133b610cfabe6d6d4b6e5eda06373bc46000cf601b661f9243db16f482156a91d7c9008ca9a1d4c501000000000000000a2a6172e08a7c0100000a6b14363931303037343761363664363235343236363600000000020000000000000000266a24aa21a9ed47542e50fcec7a7b535c2b6a35cf4ac18722ad3289d9b90d037124862db8ec3e6c9770930b0000001976a9146f5cf1be10f3ad794eca67821fb280305b2900a188ac0120000000000000000000000000000000000000000000000000000000000000000000000000", "", null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": null
}
```

