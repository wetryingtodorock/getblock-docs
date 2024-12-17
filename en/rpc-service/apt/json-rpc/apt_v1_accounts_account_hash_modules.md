---
title: apt:/v1/accounts/{account_hash}/modules \[GET\]
description: Gets all modules for a specified account and ledger version.
---

### Parameters


`limit` -

Maximum number of resources to retrieve. Gets default page size if not
provided.

`ledger_version` -

Ledger version. Defaults to latest if not provided.

`start` -

Optional cursor specifying pagination start. You can call this endpoint
once without this parameter, and then use the cursor returned in the
X-Aptos-Cursor header in the response.

### Request

``` java
curl --location --request GET 'https://apt.getblock.io/v1/accounts/0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255/modules?limit=10' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
[]
```

