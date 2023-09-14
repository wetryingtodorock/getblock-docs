---
title: xlm:/ledgers/{sequence} \[GET\]
description: The single ledger endpoint provides information on a specific ledger.
---

### Parameters


`sequence` - path

integer, optional

The sequence number of a specific ledger.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/ledgers/45678721' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_links": {
        "effects": {
            "href": "https://xlm.getblock.io/ledgers/45678721/effects{?cursor,limit,order}",
            "templated": true
        },
        "operations": {
            "href": "https://xlm.getblock.io/ledgers/45678721/operations{?cursor,limit,order}",
            "templated": true
        },
        "payments": {
            "href": "https://xlm.getblock.io/ledgers/45678721/payments{?cursor,limit,order}",
            "templated": true
        },
        "self": {
            "href": "https://xlm.getblock.io/ledgers/45678721"
        },
        "transactions": {
            "href": "https://xlm.getblock.io/ledgers/45678721/transactions{?cursor,limit,order}",
            "templated": true
        }
    },
    "base_fee_in_stroops": 100,
    "base_reserve_in_stroops": 5000000,
    "closed_at": "2023-04-04T10:14:56Z",
    "failed_transaction_count": 17,
    "fee_pool": "3678306.1969888",
    "hash": "c0744e9a2ff25b4a4ea27877aa65e2c8f3ade6a1a91a18a44d203d88266bd911",
    "header_xdr": "AAAAEySuEovXrDnv/JNEmwTCYTLjdK0Dczn9sAS813qcHVMZMgxYhjJvaiDREDxvQBQ9hkxfG8y9SRHtDaGax84sFNUAAAAAZCv4oAAAAAAAAAABAAAAAPsLErXhs5nB/PBjevRUYxi38TMxR/LbCU2ivvBEXjyTAAAAQAnCVS6SqU11pQMUQONdOpWqhEyb9wvmC6XzG13I3LPYgpuS4wCnkLQbrzaQi9NV8K9lUP6uPtd/WtewG/rhpAarZQ8xEr+QxyMQJ4SyZy3kQntJOnCDCHiQ30H9jsZ/nbXIfrMJrhS8oj3+OAjLDAyjecDJq1zpaAxK+myauiToArkAgQ6iHrPseVthAAAhdDlXq+AAAAEWAAAAAEleJmUAAABkAExLQAAAA+j9yVrmmfgOUWALZvjFjwncEVV0mVNg63xddRnSSY4gx+IHudHihq1T5HDppRYgU3eRF+uk/d3/QHxUaXtQqp5qpZiAMxv0Zk35/ASHEnAUtpU914icfL2NdipzItGdNq/V7WS4ZAhYfPzgs3v/91SvAYsHKvgB71sirU+HrFEleQAAAAA=",
    "id": "c0744e9a2ff25b4a4ea27877aa65e2c8f3ade6a1a91a18a44d203d88266bd911",
    "max_tx_set_size": 1000,
    "operation_count": 971,
    "paging_token": "196188612818108416",
    "prev_hash": "24ae128bd7ac39effc93449b04c26132e374ad037339fdb004bcd77a9c1d5319",
    "protocol_version": 19,
    "sequence": 45678721,
    "successful_transaction_count": 151,
    "total_coins": "105443902087.3472865",
    "tx_set_operation_count": 1000
}
```

