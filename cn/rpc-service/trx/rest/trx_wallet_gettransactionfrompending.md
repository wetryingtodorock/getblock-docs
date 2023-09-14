---
title: trx:/wallet/gettransactionfrompending \[POST\]
description: Get transaction details from the pending pool
---

### Parameters


`value` -

string

transaction hash

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/gettransactionfrompending' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"value": "9edf97791881d5e19fd2f04e2416ba83717cd8fa9775668fd6d79bdaeb47c6eb"}'
```

###  Response

``` java
{
  "blockNumber": 30864600,
  "blockTimeStamp": 1623056091000,
  "contractResult": [
      ""
  ],
  "id": "9edf97791881d5e19fd2f04e2416ba83717cd8fa9775668fd6d79bdaeb47c6eb",
  "receipt": {
      "net_usage": 283
  }
}
```

