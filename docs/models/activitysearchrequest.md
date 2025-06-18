# ActivitySearchRequest

Complex search request for Activities

## Example Usage

```typescript
import { ActivitySearchRequest } from "@rarible/protocol-mcp";

let value: ActivitySearchRequest = {
  filter: {
    blockchains: [
      "ETHEREUM",
    ],
    collections: [
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    ],
    items: [
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    ],
    users: {
      any: [
        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      ],
      from: [
        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      ],
      to: [
        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      ],
    },
    currencies: {
      bid: [
        "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
      ],
    },
  },
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `size`                                                           | *number*                                                         | :heavy_minus_sign:                                               | Number of entities returned                                      |
| `cursor`                                                         | *string*                                                         | :heavy_minus_sign:                                               | Cursor token to paginate Activity search result                  |
| `filter`                                                         | [models.ActivitySearchFilter](../models/activitysearchfilter.md) | :heavy_check_mark:                                               | N/A                                                              |
| `sort`                                                           | [models.ActivitySearchSort](../models/activitysearchsort.md)     | :heavy_minus_sign:                                               | N/A                                                              |