---
title: xlm:/accounts/{account_id} \[GET\]
description: The single account endpoint provides information on a specific account.The balances section in the response will also list all the trustlinesthis account has established, including trustlines that haven’t beenauthorized yet.
---

### Parameters


`account_id` - path

string, required

This account's public key encoded in a base32 string representation.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_links": {
        "data": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/data/{key}",
            "templated": true
        },
        "effects": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/effects{?cursor,limit,order}",
            "templated": true
        },
        "offers": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/offers{?cursor,limit,order}",
            "templated": true
        },
        "operations": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/operations{?cursor,limit,order}",
            "templated": true
        },
        "payments": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/payments{?cursor,limit,order}",
            "templated": true
        },
        "self": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
        },
        "trades": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/trades{?cursor,limit,order}",
            "templated": true
        },
        "transactions": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/transactions{?cursor,limit,order}",
            "templated": true
        }
    },
    "account_id": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
    "balances": [
        {
            "asset_code": "AUDV",
            "asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
            "asset_type": "credit_alphanum4",
            "balance": "1.0000000",
            "buying_liabilities": "0.0000000",
            "is_authorized": true,
            "is_authorized_to_maintain_liabilities": true,
            "last_modified_ledger": 43547513,
            "limit": "922337203685.4775807",
            "selling_liabilities": "0.0000000"
        },
        {
            "asset_code": "EURV",
            "asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
            "asset_type": "credit_alphanum4",
            "balance": "0.0000000",
            "buying_liabilities": "0.0000000",
            "is_authorized": true,
            "is_authorized_to_maintain_liabilities": true,
            "last_modified_ledger": 43165762,
            "limit": "922337203685.4775807",
            "selling_liabilities": "0.0000000"
        }
    ],
    "data": {},
    "flags": {
        "auth_clawback_enabled": false,
        "auth_immutable": false,
        "auth_required": false,
        "auth_revocable": false
    },
    "home_domain": "lobstr.co",
    "id": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
    "inflation_destination": "GDCHDRSDOBRMSUDKRE2C4U4KDLNEATJPIHHR2ORFL5BSD56G4DQXL4VW",
    "last_modified_ledger": 46844540,
    "last_modified_time": "2023-06-20T19:46:04Z",
    "num_sponsored": 0,
    "num_sponsoring": 0,
    "paging_token": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
    "sequence": "185387470148735007",
    "sequence_ledger": 46844540,
    "sequence_time": "1687290364",
    "signers": [
        {
            "key": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
            "type": "ed25519_public_key",
            "weight": 1
        }
    ],
    "subentry_count": 15,
    "thresholds": {
        "high_threshold": 0,
        "low_threshold": 0,
        "med_threshold": 0
    }
}
```

