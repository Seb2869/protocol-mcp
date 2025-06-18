# OlapUserLeaderboardEntry

## Example Usage

```typescript
import { OlapUserLeaderboardEntry } from "@rarible/protocol-mcp";

let value: OlapUserLeaderboardEntry = {
  id: "<id>",
  volumeUsd: {
    value: 9404.89,
  },
  volumeNative: {
    value: 7159.42,
  },
  items: 480617,
  transactions: 795043,
};
```

## Fields

| Field                                                        | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `id`                                                         | *string*                                                     | :heavy_check_mark:                                           | Identifier of user                                           |
| `volumeUsd`                                                  | [models.OlapCurrencyAmount](../models/olapcurrencyamount.md) | :heavy_check_mark:                                           | N/A                                                          |
| `volumeNative`                                               | [models.OlapCurrencyAmount](../models/olapcurrencyamount.md) | :heavy_check_mark:                                           | N/A                                                          |
| `items`                                                      | *number*                                                     | :heavy_check_mark:                                           | (non-unique) amount of traded items                          |
| `transactions`                                               | *number*                                                     | :heavy_check_mark:                                           | Amount of transactions were made                             |