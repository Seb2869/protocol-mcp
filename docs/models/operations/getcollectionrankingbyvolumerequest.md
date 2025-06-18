# GetCollectionRankingByVolumeRequest

## Example Usage

```typescript
import { GetCollectionRankingByVolumeRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetCollectionRankingByVolumeRequest = {};
```

## Fields

| Field                                                                                       | Type                                                                                        | Required                                                                                    | Description                                                                                 |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| `source`                                                                                    | [models.OlapTradesLeaderboardSourceGroup](../../models/olaptradesleaderboardsourcegroup.md) | :heavy_minus_sign:                                                                          | Group of platform used for volume calculation and collection ranging.                       |
| `blockchain`                                                                                | [models.OlapBlockchain](../../models/olapblockchain.md)                                     | :heavy_minus_sign:                                                                          | Blockchain                                                                                  |
| `ids`                                                                                       | *string*[]                                                                                  | :heavy_minus_sign:                                                                          | Collection ids                                                                              |
| `period`                                                                                    | [models.OlapLeaderboardPeriod](../../models/olapleaderboardperiod.md)                       | :heavy_minus_sign:                                                                          | Time period for aggregation                                                                 |
| `minFloorPriceNative`                                                                       | *number*                                                                                    | :heavy_minus_sign:                                                                          | Show collections which floor price (native currency) more or equal than specified value     |
| `maxFloorPriceNative`                                                                       | *number*                                                                                    | :heavy_minus_sign:                                                                          | Show collections which floor price (native currency) less or equal than specified value     |
| `sort`                                                                                      | [models.OlapTradesLeaderboardSort](../../models/olaptradesleaderboardsort.md)               | :heavy_minus_sign:                                                                          | Collections sorting                                                                         |
| `limit`                                                                                     | *number*                                                                                    | :heavy_minus_sign:                                                                          | Limit of records in leaderboard                                                             |
| `continuation`                                                                              | *string*                                                                                    | :heavy_minus_sign:                                                                          | Page reference. Taken from previous response                                                |