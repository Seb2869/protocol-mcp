# OlapBidsByPrice

## Example Usage

```typescript
import { OlapBidsByPrice } from "@rarible/protocol-mcp";

let value: OlapBidsByPrice = {
  price: 7478.73,
  bidsCount: 729081,
  volumeNative: 1629.08,
  buyersCount: 417515,
  buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      | Example                                                          |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `price`                                                          | *number*                                                         | :heavy_check_mark:                                               | N/A                                                              |                                                                  |
| `bidsCount`                                                      | *number*                                                         | :heavy_check_mark:                                               | N/A                                                              |                                                                  |
| `volumeNative`                                                   | *number*                                                         | :heavy_check_mark:                                               | N/A                                                              |                                                                  |
| `buyersCount`                                                    | *number*                                                         | :heavy_check_mark:                                               | N/A                                                              |                                                                  |
| `buyer`                                                          | *string*                                                         | :heavy_minus_sign:                                               | Blockchain address in Union format `${blockchainGroup}:${token}` | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb              |