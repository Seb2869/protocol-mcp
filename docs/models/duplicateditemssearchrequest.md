# DuplicatedItemsSearchRequest

Search request for items with duplicated traits

## Example Usage

```typescript
import { DuplicatedItemsSearchRequest } from "@rarible/protocol-mcp";

let value: DuplicatedItemsSearchRequest = {
  filter: {
    blockchains: [
      "ETHEREUM",
    ],
    collections: [
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    ],
    traits: [
      {
        key: "Hat",
        value: "Halo",
      },
    ],
    traitRanges: [
      {
        key: "Hat",
        valueRange: {},
      },
    ],
    creators: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    owners: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    mintedAtFrom: new Date("2021-08-25T00:00:00Z"),
    mintedAtTo: new Date("2029-12-01T00:00:00Z"),
    lastUpdatedAtFrom: new Date("2021-08-25T00:00:00Z"),
    lastUpdatedAtTo: new Date("2029-12-01T00:00:00Z"),
    sellPriceFrom: 0,
    sellPriceTo: 999999,
    sellCurrency: "ETHEREUM:0x0000000000000000000000000000000000000000",
    bidPriceFrom: 0,
    bidPriceTo: 999999,
    bidCurrency: "ETHEREUM:0x0000000000000000000000000000000000000000",
  },
  traits: [
    "<value>",
  ],
};
```

## Fields

| Field                                                      | Type                                                       | Required                                                   | Description                                                |
| ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- |
| `size`                                                     | *number*                                                   | :heavy_minus_sign:                                         | Number of entities returned                                |
| `continuation`                                             | *string*                                                   | :heavy_minus_sign:                                         | Continuation token to paginate items search result         |
| `filter`                                                   | [models.ItemsSearchFilter](../models/itemssearchfilter.md) | :heavy_check_mark:                                         | Filter for items search query                              |
| `traits`                                                   | *string*[]                                                 | :heavy_check_mark:                                         | Traits names to group by                                   |