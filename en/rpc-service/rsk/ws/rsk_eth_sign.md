---
title: rsk:eth_sign \[WebSocket\]
description: The sign method calculates an Ethereum specific signature withsign(keccak256(\x19Ethereum Signed Message\n + len(message) +message))).By adding a prefix to the message makes the calculated signaturerecognisable as an Ethereum specific signature. This prevents misusewhere a malicious DApp can sign arbitrary data (e.g. transaction) anduse the signature to impersonate the victim.Note the address to sign with must be unlocked.
---

### Parameters


`DATA` - string

address.

`DATA` - string

message to sign.

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0x9b2055d370f73ec7d8a03e965129118dc8f5bf83", "0xdeadbeaf"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xa3f20717a250c2b0b729b7e5becbff67fdaef7e0699da4de7ca5895b02a170a12d887fd3b17bfdce3481f10bea41f45ba9f709d39ce8325427b57afcfc994cee1b"
}
```

