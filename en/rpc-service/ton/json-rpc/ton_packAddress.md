---
title: ton:/packAddress \[GET\]
description: Convert an address from raw to human-readable format.
---

### Parameters


`address` - query

required, string

Identifier of target TON account in any form.

### Request

``` java
curl --location --request GET 'https://ton.getblock.io/mainnet/packAddress?address=0:d76767392e7035d84ba6f83960b9399f62430ebcd7850a1e2b043d2d826c2370' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "ok": true,
    "result": "EQDXZ2c5LnA12Eum+DlguTmfYkMOvNeFCh4rBD0tgmwjcFI+"
}
```

