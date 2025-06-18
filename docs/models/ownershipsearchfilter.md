# OwnershipSearchFilter

Filter for ownerships search query

## Example Usage

```typescript
import { OwnershipSearchFilter } from "@rarible/protocol-mcp";

let value: OwnershipSearchFilter = {
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
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `blockchains`                                                                                 | [models.Blockchain](../models/blockchain.md)[]                                                | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `owners`                                                                                      | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `collections`                                                                                 | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `items`                                                                                       | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `beforeDate`                                                                                  | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `afterDate`                                                                                   | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `sellPriceFrom`                                                                               | *number*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `sellPriceTo`                                                                                 | *number*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `sellCurrency`                                                                                | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `sellPlatforms`                                                                               | [models.Platform](../models/platform.md)[]                                                    | :heavy_minus_sign:                                                                            | N/A                                                                                           |