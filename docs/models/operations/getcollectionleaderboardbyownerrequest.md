# GetCollectionLeaderboardByOwnerRequest

## Example Usage

```typescript
import { GetCollectionLeaderboardByOwnerRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetCollectionLeaderboardByOwnerRequest = {
  owners: [
    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  ],
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `owners`                                                                            | *string*[]                                                                          | :heavy_check_mark:                                                                  | Addresses of the owner                                                              |
| `blockchains`                                                                       | [models.OlapBlockchain](../../models/olapblockchain.md)[]                           | :heavy_minus_sign:                                                                  | Blockchain networks                                                                 |
| `period`                                                                            | [models.OlapPeriod](../../models/olapperiod.md)                                     | :heavy_minus_sign:                                                                  | Time period for aggregation                                                         |
| `sort`                                                                              | [models.OlapLeaderboardSort](../../models/olapleaderboardsort.md)                   | :heavy_minus_sign:                                                                  | Collections sorting                                                                 |
| `direction`                                                                         | [models.OlapLeaderboardSortDirection](../../models/olapleaderboardsortdirection.md) | :heavy_minus_sign:                                                                  | Collections sorting direction                                                       |
| `limit`                                                                             | *number*                                                                            | :heavy_minus_sign:                                                                  | Limit of records in leaderboard                                                     |
| `continuation`                                                                      | *string*                                                                            | :heavy_minus_sign:                                                                  | Continuation token from the previous response                                       |