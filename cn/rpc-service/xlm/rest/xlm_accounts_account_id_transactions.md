---
title: xlm:/accounts/{account_id}/transactions \[GET\]
description: This endpoint represents successful transactions for a given account andcan be used in streaming mode. Streaming mode allows you to listen fornew transactions for this account as they are added to the Stellarledger. If called in streaming mode, Horizon will start at the earliestknown transaction unless a cursor is set, in which case it will startfrom that cursor. By setting the cursor value to now, you can streamtransactions created since your request time.
---

### Parameters


`account_id` - path

string, required

This account's public key encoded in a base32 string representation.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

Possible values: \[asc, desc\], optional

A designation of the order in which records should appear. Options
include asc (ascending) or desc (descending). If this argument isn’t
set, it defaults to asc.

`limit` - query

integer, optional

The maximum number of records returned. The limit can range from 1 to
200 - an upper limit that is hardcoded in Horizon for performance
reasons. If this argument isn’t designated, it defaults to 10.

`include_failed` - query

boolean, optional

Set to true to include failed operations in results. Options include
true and false.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/transactions?limit=5' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_embedded": {
        "records": [
            {
                "_links": {
                    "account": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
                    },
                    "effects": {
                        "href": "https://xlm.getblock.io/transactions/754b492c09963177def246f02e66452b6c9bf2532cb1b00cd5691d34ae408747/effects{?cursor,limit,order}",
                        "templated": true
                    },
                    "ledger": {
                        "href": "https://xlm.getblock.io/ledgers/45678723"
                    },
                    "operations": {
                        "href": "https://xlm.getblock.io/transactions/754b492c09963177def246f02e66452b6c9bf2532cb1b00cd5691d34ae408747/operations{?cursor,limit,order}",
                        "templated": true
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/transactions?order=asc&cursor=196188621408321536"
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/transactions/754b492c09963177def246f02e66452b6c9bf2532cb1b00cd5691d34ae408747"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/transactions?order=desc&cursor=196188621408321536"
                    },
                    "transaction": {
                        "href": "https://xlm.getblock.io/transactions/754b492c09963177def246f02e66452b6c9bf2532cb1b00cd5691d34ae408747"
                    }
                },
                "created_at": "2023-04-04T10:15:07Z",
                "envelope_xdr": "AAAAAgAAAACQrJoUoYGFW7WOt8Kdq4tNBAxtE1+JopP5DWVhQwA8ZQAAJxACkqDsAAP7XgAAAAEAAAAAAAAAAAAAAABkK/jCAAAAAAAAAAEAAAAAAAAAAwAAAAFVU0RWAAAAAMPsuTzzByJGsz6D9/hcWQFqboNOVvoUkYuIOv/8pwEEAAAAAUdCUFYAAAAAw+y5PPMHIkazPoP3+FxZAWpug05W+hSRi4g6//ynAQQAAAAAAAAAAAB6RBUAmJaAAAAAAEleIZ8AAAAAAAAAAUMAPGUAAABARZYDwGRef3QJm64KPLd0YRPosSAlVFHOdrt14E2cDJ2VuXPYLs3SIvgsSfkADUf8NdhV4fh+qwcsYlK7d1djDQ==",
                "fee_account": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                "fee_charged": "100",
                "fee_meta_xdr": "AAAAAgAAAAMCuQCAAAAAAAAAAACQrJoUoYGFW7WOt8Kdq4tNBAxtE1+JopP5DWVhQwA8ZQAAAABrKWlEApKg7AAD+10AAAAOAAAAAQAAAADEccZDcGLJUGqJNC5TihraQE0vQc8dOiVfQyH3xuDhdQAAAAAAAAAJbG9ic3RyLmNvAAAAAQAAAAAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAIAAAAAAAAAAAAAAAAAAAADAAAAAAK5AH0AAAAAZCv4igAAAAAAAAABArkAgwAAAAAAAAAAkKyaFKGBhVu1jrfCnauLTQQMbRNfiaKT+Q1lYUMAPGUAAAAAaylo4AKSoOwAA/tdAAAADgAAAAEAAAAAxHHGQ3BiyVBqiTQuU4oa2kBNL0HPHTolX0Mh98bg4XUAAAAAAAAACWxvYnN0ci5jbwAAAAEAAAAAAAAAAAAAAQAAAAAAAAAAAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAwAAAAACuQB9AAAAAGQr+IoAAAAA",
                "hash": "754b492c09963177def246f02e66452b6c9bf2532cb1b00cd5691d34ae408747",
                "id": "754b492c09963177def246f02e66452b6c9bf2532cb1b00cd5691d34ae408747",
                "ledger": 45678723,
                "max_fee": "10000",
                "memo_type": "none",
                "operation_count": 1,
                "paging_token": "196188621408321536",
                "preconditions": {
                    "timebounds": {
                        "max_time": "1680603330",
                        "min_time": "0"
                    }
                },
                "result_meta_xdr": "AAAAAgAAAAIAAAADArkAgwAAAAAAAAAAkKyaFKGBhVu1jrfCnauLTQQMbRNfiaKT+Q1lYUMAPGUAAAAAaylo4AKSoOwAA/tdAAAADgAAAAEAAAAAxHHGQ3BiyVBqiTQuU4oa2kBNL0HPHTolX0Mh98bg4XUAAAAAAAAACWxvYnN0ci5jbwAAAAEAAAAAAAAAAAAAAQAAAAAAAAAAAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAwAAAAACuQB9AAAAAGQr+IoAAAAAAAAAAQK5AIMAAAAAAAAAAJCsmhShgYVbtY63wp2ri00EDG0TX4mik/kNZWFDADxlAAAAAGspaOACkqDsAAP7XgAAAA4AAAABAAAAAMRxxkNwYslQaok0LlOKGtpATS9Bzx06JV9DIffG4OF1AAAAAAAAAAlsb2JzdHIuY28AAAABAAAAAAAAAAAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAgAAAAAAAAAAAAAAAAAAAAMAAAAAArkAgwAAAABkK/irAAAAAAAAAAEAAAAIAAAAAwK5AG4AAAACAAAAAJCsmhShgYVbtY63wp2ri00EDG0TX4mik/kNZWFDADxlAAAAAEleIZ8AAAABVVNEVgAAAADD7Lk88wciRrM+g/f4XFkBam6DTlb6FJGLiDr//KcBBAAAAAFHQlBWAAAAAMPsuTzzByJGsz6D9/hcWQFqboNOVvoUkYuIOv/8pwEEAAAACXGQfAAAAAB9AAAAnAAAAAAAAAAAAAAAAAAAAAIAAAACAAAAAJCsmhShgYVbtY63wp2ri00EDG0TX4mik/kNZWFDADxlAAAAAEleIZ8AAAADArkAgwAAAAEAAAAAkKyaFKGBhVu1jrfCnauLTQQMbRNfiaKT+Q1lYUMAPGUAAAABR0JQVgAAAADD7Lk88wciRrM+g/f4XFkBam6DTlb6FJGLiDr//KcBBAAAAIMfj5jif/////////8AAAABAAAAAQAAACUeM2+kAAAAITJuJQAAAAAAAAAAAAAAAAECuQCDAAAAAQAAAACQrJoUoYGFW7WOt8Kdq4tNBAxtE1+JopP5DWVhQwA8ZQAAAAFHQlBWAAAAAMPsuTzzByJGsz6D9/hcWQFqboNOVvoUkYuIOv/8pwEEAAAAgx+PmOJ//////////wAAAAEAAAABAAAAHY0MyqQAAAAhMm4lAAAAAAAAAAAAAAAAAwK5AIMAAAAAAAAAAJCsmhShgYVbtY63wp2ri00EDG0TX4mik/kNZWFDADxlAAAAAGspaOACkqDsAAP7XgAAAA4AAAABAAAAAMRxxkNwYslQaok0LlOKGtpATS9Bzx06JV9DIffG4OF1AAAAAAAAAAlsb2JzdHIuY28AAAABAAAAAAAAAAAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAgAAAAAAAAAAAAAAAAAAAAMAAAAAArkAgwAAAABkK/irAAAAAAAAAAECuQCDAAAAAAAAAACQrJoUoYGFW7WOt8Kdq4tNBAxtE1+JopP5DWVhQwA8ZQAAAABrKWjgApKg7AAD+14AAAANAAAAAQAAAADEccZDcGLJUGqJNC5TihraQE0vQc8dOiVfQyH3xuDhdQAAAAAAAAAJbG9ic3RyLmNvAAAAAQAAAAAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAIAAAAAAAAAAAAAAAAAAAADAAAAAAK5AIMAAAAAZCv4qwAAAAAAAAADArkAgwAAAAEAAAAAkKyaFKGBhVu1jrfCnauLTQQMbRNfiaKT+Q1lYUMAPGUAAAABVVNEVgAAAADD7Lk88wciRrM+g/f4XFkBam6DTlb6FJGLiDr//KcBBAAAAJSeDR9Pf/////////8AAAABAAAAAQAAACmHNCKAAAAALls7ATsAAAAAAAAAAAAAAAECuQCDAAAAAQAAAACQrJoUoYGFW7WOt8Kdq4tNBAxtE1+JopP5DWVhQwA8ZQAAAAFVU0RWAAAAAMPsuTzzByJGsz6D9/hcWQFqboNOVvoUkYuIOv/8pwEEAAAAlJ4NH09//////////wAAAAEAAAABAAAAKYc0IoAAAAAk6aqFOwAAAAAAAAAAAAAAAA==",
                "result_xdr": "AAAAAAAAAGQAAAAAAAAAAQAAAAAAAAADAAAAAAAAAAAAAAACAAAAAA==",
                "signatures": [
                    "RZYDwGRef3QJm64KPLd0YRPosSAlVFHOdrt14E2cDJ2VuXPYLs3SIvgsSfkADUf8NdhV4fh+qwcsYlK7d1djDQ=="
                ],
                "source_account": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                "source_account_sequence": "185387470148598622",
                "successful": true,
                "valid_after": "1970-01-01T00:00:00Z",
                "valid_before": "2023-04-04T10:15:30Z"
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/transactions?cursor=196188754552455168&limit=5&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/transactions?cursor=196188621408321536&limit=5&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/transactions?cursor=&limit=5&order=asc"
        }
    }
}
```

