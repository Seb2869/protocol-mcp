# OrderActivityMatchSide

## Example Usage

```typescript
import { OrderActivityMatchSide } from "@rarible/protocol-mcp";

let value: OrderActivityMatchSide = {
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  asset: {
    type: {
      atType: "SOLANA_SOL",
    },
    value: "123456.789",
  },
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      | Example                                                          |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `maker`                                                          | *string*                                                         | :heavy_check_mark:                                               | Blockchain address in Union format `${blockchainGroup}:${token}` | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb              |
| `hash`                                                           | *string*                                                         | :heavy_minus_sign:                                               | N/A                                                              |                                                                  |
| `asset`                                                          | [models.Asset](../models/asset.md)                               | :heavy_check_mark:                                               | N/A                                                              |                                                                  |