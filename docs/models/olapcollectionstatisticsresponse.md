# OlapCollectionStatisticsResponse

## Example Usage

```typescript
import { OlapCollectionStatisticsResponse } from "@rarible/protocol-mcp";

let value: OlapCollectionStatisticsResponse = {
  highestSale: [
    {
      value: 8715.11,
    },
  ],
  floorPrice: [
    {
      value: 6442.24,
    },
  ],
  marketCap: [
    {
      value: 3348.33,
    },
  ],
  volume: [
    {
      value: 6250.76,
    },
  ],
  listed: 408165,
  items: 855922,
  owners: 189703,
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `highestSale`                                                          | [models.OlapCurrencyAmount](../models/olapcurrencyamount.md)[]         | :heavy_check_mark:                                                     | Highest worth transaction in collection                                |
| `floorPrice`                                                           | [models.OlapCurrencyAmount](../models/olapcurrencyamount.md)[]         | :heavy_check_mark:                                                     | Minimal price of nft in this collection available on rarible           |
| `marketCap`                                                            | [models.OlapCurrencyAmount](../models/olapcurrencyamount.md)[]         | :heavy_check_mark:                                                     | Market cap of collection (floor price * total item supply)             |
| `volume`                                                               | [models.OlapCurrencyAmount](../models/olapcurrencyamount.md)[]         | :heavy_check_mark:                                                     | Total worth of all transactions were made with nfts in this collection |
| `listed`                                                               | *number*                                                               | :heavy_check_mark:                                                     | Amount of currently listed items                                       |
| `items`                                                                | *number*                                                               | :heavy_check_mark:                                                     | Total item supply of all nfts in the collection                        |
| `owners`                                                               | *number*                                                               | :heavy_check_mark:                                                     | Current amount of unique owners who hold nfts of this collection       |