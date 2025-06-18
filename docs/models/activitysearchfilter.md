# ActivitySearchFilter

## Example Usage

```typescript
import { ActivitySearchFilter } from "@rarible/protocol-mcp";

let value: ActivitySearchFilter = {
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
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `blockchains`                                                                                 | [models.Blockchain](../models/blockchain.md)[]                                                | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `types`                                                                                       | [models.ActivityType](../models/activitytype.md)[]                                            | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `collections`                                                                                 | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `items`                                                                                       | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `users`                                                                                       | [models.ActivityUserFilter](../models/activityuserfilter.md)                                  | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `currencies`                                                                                  | [models.ActivityCurrencyFilter](../models/activitycurrencyfilter.md)                          | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `from`                                                                                        | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `to`                                                                                          | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `fromBlockInclusive`                                                                          | *number*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `toBlockExclusive`                                                                            | *number*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |