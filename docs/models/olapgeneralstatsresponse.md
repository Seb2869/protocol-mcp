# OlapGeneralStatsResponse

## Example Usage

```typescript
import { OlapGeneralStatsResponse } from "@rarible/protocol-mcp";

let value: OlapGeneralStatsResponse = {
  highestSale: 8017.21,
  listed: 403296,
  items: 654214,
  owners: 220793,
  volume: 5970.07,
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `highestSale`                                                          | *number*                                                               | :heavy_check_mark:                                                     | Highest worth transaction in collection                                |
| `floorPrice`                                                           | *number*                                                               | :heavy_minus_sign:                                                     | Minimal price of nft in this collection available on rarible           |
| `marketCap`                                                            | *number*                                                               | :heavy_minus_sign:                                                     | Market cap of collection (floor price * total item supply)             |
| `listed`                                                               | *number*                                                               | :heavy_check_mark:                                                     | Amount of currently listed items                                       |
| `items`                                                                | *number*                                                               | :heavy_check_mark:                                                     | Total item supply of all nfts in the collection                        |
| `owners`                                                               | *number*                                                               | :heavy_check_mark:                                                     | Current amount of unique owners who hold nfts of this collection       |
| `volume`                                                               | *number*                                                               | :heavy_check_mark:                                                     | Total worth of all transactions were made with nfts in this collection |