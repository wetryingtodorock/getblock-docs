---
title: btg:fundrawtransaction \[POST\]
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
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "fundrawtransaction",
"params": ["hexstring", "", null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "010000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff1b035025390485393661087ddf058133cfb60008694f6f417068647100000000020065cd1d0000000017a914875ff5ac568b44a58b7f71df71e6d8288725a9a7870000000000000000266a24aa21a9ede2f61c3f71d1defd3fa999dfa36953755c690689799962b48bebd836974e8cf90120000000000000000000000000000000000000000000000000000000000000000000000000"
}
```

