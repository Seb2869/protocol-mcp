# OlapCollectionLeaderboardItem

## Example Usage

```typescript
import { OlapCollectionLeaderboardItem } from "@rarible/protocol-mcp";

let value: OlapCollectionLeaderboardItem = {
  id: "<id>",
  sales: 348874,
  volume: {
    currency: "Armenian Dram",
    value: 4362.82,
  },
  floorHistory: {
    timestamps: [
      485634,
    ],
    values: [
      7962.99,
    ],
  },
  globalStats: {
    listed: 572933,
    items: 356769,
    owners: 140220,
  },
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `id`                                                                                           | *string*                                                                                       | :heavy_check_mark:                                                                             | Identifier of collection                                                                       |
| `sales`                                                                                        | *number*                                                                                       | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `volume`                                                                                       | [models.OlapPriceWithUsd](../models/olappricewithusd.md)                                       | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `floorChangePercent`                                                                           | *number*                                                                                       | :heavy_minus_sign:                                                                             | N/A                                                                                            |
| `floorHistory`                                                                                 | [models.OlapHistoryValuesByTimestamps](../models/olaphistoryvaluesbytimestamps.md)             | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `globalStats`                                                                                  | [models.OlapCollectionLeaderboardStatistics](../models/olapcollectionleaderboardstatistics.md) | :heavy_check_mark:                                                                             | N/A                                                                                            |