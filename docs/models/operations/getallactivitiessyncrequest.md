# GetAllActivitiesSyncRequest

## Example Usage

```typescript
import { GetAllActivitiesSyncRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetAllActivitiesSyncRequest = {
  blockchain: "ETHEREUM",
};
```

## Fields

| Field                                           | Type                                            | Required                                        | Description                                     | Example                                         |
| ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| `blockchain`                                    | [models.Blockchain](../../models/blockchain.md) | :heavy_check_mark:                              | Type of the blockchain network                  | ETHEREUM                                        |
| `continuation`                                  | *string*                                        | :heavy_minus_sign:                              | Continuation token from the previous response   |                                                 |
| `size`                                          | *number*                                        | :heavy_minus_sign:                              | The number of items to return                   |                                                 |
| `sort`                                          | [models.SyncSort](../../models/syncsort.md)     | :heavy_minus_sign:                              | Sorting by data base update time                |                                                 |
| `type`                                          | [models.SyncType](../../models/synctype.md)     | :heavy_minus_sign:                              | Filtering by activity type                      |                                                 |