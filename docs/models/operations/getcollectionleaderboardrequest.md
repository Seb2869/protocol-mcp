# GetCollectionLeaderboardRequest

## Example Usage

```typescript
import { GetCollectionLeaderboardRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetCollectionLeaderboardRequest = {};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `blockchains`                                                                       | [models.OlapBlockchain](../../models/olapblockchain.md)[]                           | :heavy_minus_sign:                                                                  | Blockchain networks                                                                 |
| `period`                                                                            | [models.OlapPeriod](../../models/olapperiod.md)                                     | :heavy_minus_sign:                                                                  | Time period for aggregation                                                         |
| `sort`                                                                              | [models.OlapLeaderboardSort](../../models/olapleaderboardsort.md)                   | :heavy_minus_sign:                                                                  | Collections sorting                                                                 |
| `direction`                                                                         | [models.OlapLeaderboardSortDirection](../../models/olapleaderboardsortdirection.md) | :heavy_minus_sign:                                                                  | Collections sorting direction                                                       |
| `limit`                                                                             | *number*                                                                            | :heavy_minus_sign:                                                                  | Limit of records in leaderboard                                                     |
| `offset`                                                                            | *number*                                                                            | :heavy_minus_sign:                                                                  | Offset reference                                                                    |