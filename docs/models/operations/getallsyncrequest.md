# GetAllSyncRequest

## Example Usage

```typescript
import { GetAllSyncRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetAllSyncRequest = {
  blockchain: "ETHEREUM",
};
```

## Fields

| Field                                           | Type                                            | Required                                        | Description                                     | Example                                         |
| ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| `blockchain`                                    | [models.Blockchain](../../models/blockchain.md) | :heavy_check_mark:                              | Type of the blockchain network                  | ETHEREUM                                        |
| `continuation`                                  | *string*                                        | :heavy_minus_sign:                              | Continuation token from the previous response   |                                                 |
| `size`                                          | *number*                                        | :heavy_minus_sign:                              | The number of orders to return                  |                                                 |
| `sort`                                          | [models.SyncSort](../../models/syncsort.md)     | :heavy_minus_sign:                              | Order sort                                      |                                                 |