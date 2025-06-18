# GetUserRankingByVolumeRequest

## Example Usage

```typescript
import { GetUserRankingByVolumeRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetUserRankingByVolumeRequest = {
  entity: "buyers",
};
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `entity`                                                              | [models.OlapUserType](../../models/olapusertype.md)                   | :heavy_check_mark:                                                    | Type of users in leaderboard                                          |
| `blockchain`                                                          | [models.OlapBlockchain](../../models/olapblockchain.md)               | :heavy_minus_sign:                                                    | Blockchain                                                            |
| `source`                                                              | [models.OlapPlatformSource](../../models/olapplatformsource.md)       | :heavy_minus_sign:                                                    | Source                                                                |
| `period`                                                              | [models.OlapLeaderboardPeriod](../../models/olapleaderboardperiod.md) | :heavy_minus_sign:                                                    | Time period of leaderboard. Default: D7                               |
| `limit`                                                               | *number*                                                              | :heavy_minus_sign:                                                    | Limit of records in leaderboard                                       |