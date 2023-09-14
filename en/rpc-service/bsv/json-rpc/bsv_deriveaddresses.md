---
title: bsv:deriveaddresses \[POST\]
description: Derives one or more addresses corresponding to an output descriptor.In the above, pubkey either refers to a fixed public key in hexadecimalnotation, or to an xpub/xprv optionally followed by one or more pathelements separated by /, where h represents a hardened child key.For more information on output descriptors, see the documentation in thedoc/descriptors.md file.
---

### Parameters


`descriptor` - string, required

The descriptor.

`range` - numeric or array, optional

If a ranged descriptor is used, this specifies the end or the range (in
\[begin,end\] notation) to derive.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "sendrawtransaction",
"params": ["descriptor", null],
"id": "getblock.io"}'
```

