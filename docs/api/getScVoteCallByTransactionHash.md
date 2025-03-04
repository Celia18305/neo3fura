# GetScVoteCallByTransactionHash
Gets the Scvote call by transaction hash
<hr>

### Request

> POST https://testneofura.ngd.network:444

#### Body Parameters
|    Name    | Type | Description | Required |
| ---------- | --- |    ------    | ----|
| TransactionHash     | string|  the transactionHash| required|


#### Example
```
curl --location --request POST 'https://testneofura.ngd.network:444' \
--header 'Content-Type: application/json' \
--data-raw '{  
  "jsonrpc": "2.0",
  "method": "GetScVoteCallByTransactionHash",
  "params": {"TransactionHash":"0x3d07e51614efd0d6eeeb1de7da6ce5b2f1db61a901e10b9c6715de5add0888fc" },
  "id": 1
}'
```
### Response
```json5
{
    "id": 1,
        "result": {
        "_id": "614befeda14111843552202c",
            "blockNumber": 3957,
            "candidate": "0x0bf916d727c75f2e51e1ab2c476304513da59701",
            "candidatePubKey": "023e9b32ea89b94d066e649b124fd50e396ee91369e8e2a6ae1b11c170d022256d",
            "txid": "0x3d07e51614efd0d6eeeb1de7da6ce5b2f1db61a901e10b9c6715de5add0888fc",
            "voter": "0x0bf916d727c75f2e51e1ab2c476304513da59701"
    },
    "error": null
}
```
