# ItemTransfer

## Example Usage

```typescript
import { ItemTransfer } from "@rarible/protocol-mcp";

let value: ItemTransfer = {
  atType: "TRANSFER",
  from: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      | Example                                                          |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `atType`                                                         | [models.ItemTransferAtType](../models/itemtransferattype.md)     | :heavy_check_mark:                                               | N/A                                                              |                                                                  |
| `from`                                                           | *string*                                                         | :heavy_check_mark:                                               | Blockchain address in Union format `${blockchainGroup}:${token}` | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb              |