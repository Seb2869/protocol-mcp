# OwnershipSearchRequest

Ownerships complex search query

## Example Usage

```typescript
import { OwnershipSearchRequest } from "@rarible/protocol-mcp";

let value: OwnershipSearchRequest = {
  filter: {
    blockchains: [
      "ETHEREUM",
    ],
    owners: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    collections: [
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    ],
    items: [
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    ],
  },
};
```

## Fields

| Field                                                              | Type                                                               | Required                                                           | Description                                                        |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `size`                                                             | *number*                                                           | :heavy_minus_sign:                                                 | Number of entities returned                                        |
| `continuation`                                                     | *string*                                                           | :heavy_minus_sign:                                                 | Continuation token to paginate ownerships search result            |
| `filter`                                                           | [models.OwnershipSearchFilter](../models/ownershipsearchfilter.md) | :heavy_check_mark:                                                 | Filter for ownerships search query                                 |
| `sort`                                                             | [models.OwnershipSearchSort](../models/ownershipsearchsort.md)     | :heavy_minus_sign:                                                 | N/A                                                                |