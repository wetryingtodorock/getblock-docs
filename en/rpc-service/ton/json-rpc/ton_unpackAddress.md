---
title: ton:/unpackAddress \[GET\]
description: Convert an address from human-readable to raw format.
---

### Parameters


`address` - query

required, string

Identifier of target TON account in any form.

### Request

``` java
curl --location --request GET 'https://ton.getblock.io/mainnet/unpackAddress?address=EQDXZ2c5LnA12Eum-DlguTmfYkMOvNeFCh4rBD0tgmwjcFI-' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "ok": true,
    "result": "0:d76767392e7035d84ba6f83960b9399f62430ebcd7850a1e2b043d2d826c2370"
}
```

