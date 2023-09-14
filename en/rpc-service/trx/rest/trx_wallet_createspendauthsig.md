---
title: trx:/wallet/createspendauthsig \[POST\] {disallowed}
description: Note To ensure security, Trongrid has disabled this interface service,please use the service provided by the local node.
---

### Parameters


`ask` - string, required.

`tx_hash` - string, required.

`aplha` - string, required.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/createspendauthsig' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

