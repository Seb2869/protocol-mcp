# EncodedEthOrder

## Example Usage

```typescript
import { EncodedEthOrder } from "@rarible/protocol-mcp";

let value: EncodedEthOrder = {
  orderHash: "<value>",
  signHash: "<value>",
  transferProxy: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  blockchain: "ETHEREUM",
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      | Example                                                          |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `atType`                                                         | [models.EncodedOrderAtType](../models/encodedorderattype.md)     | :heavy_minus_sign:                                               | N/A                                                              |                                                                  |
| `orderHash`                                                      | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              |                                                                  |
| `signHash`                                                       | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              |                                                                  |
| `transferProxy`                                                  | *string*                                                         | :heavy_minus_sign:                                               | Blockchain address in Union format `${blockchainGroup}:${token}` | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb              |
| `blockchain`                                                     | [models.Blockchain](../models/blockchain.md)                     | :heavy_check_mark:                                               | N/A                                                              | ETHEREUM                                                         |