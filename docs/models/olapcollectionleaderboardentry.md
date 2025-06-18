# OlapCollectionLeaderboardEntry

## Example Usage

```typescript
import { OlapCollectionLeaderboardEntry } from "@rarible/protocol-mcp";

let value: OlapCollectionLeaderboardEntry = {
  id: "<id>",
  volumeUsd: {
    value: 4289.8,
  },
  volumeNative: {
    value: 1106.23,
  },
  itemsBought: 651421,
  listed: 971591,
  totalItemSupply: 238713,
  ownersCount: 398069,
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `id`                                                                             | *string*                                                                         | :heavy_check_mark:                                                               | Identifier of collection                                                         |
| `volumeUsd`                                                                      | [models.OlapCurrencyAmountWithChange](../models/olapcurrencyamountwithchange.md) | :heavy_check_mark:                                                               | N/A                                                                              |
| `volumeNative`                                                                   | [models.OlapCurrencyAmount](../models/olapcurrencyamount.md)                     | :heavy_check_mark:                                                               | N/A                                                                              |
| `itemsBought`                                                                    | *number*                                                                         | :heavy_check_mark:                                                               | N/A                                                                              |
| `floorPrice`                                                                     | [models.OlapCurrencyAmountWithChange](../models/olapcurrencyamountwithchange.md) | :heavy_minus_sign:                                                               | N/A                                                                              |
| `listed`                                                                         | *number*                                                                         | :heavy_check_mark:                                                               | N/A                                                                              |
| `totalItemSupply`                                                                | *number*                                                                         | :heavy_check_mark:                                                               | N/A                                                                              |
| `ownersCount`                                                                    | *number*                                                                         | :heavy_check_mark:                                                               | N/A                                                                              |