# Creator

## Example Usage

```typescript
import { Creator } from "@rarible/protocol-mcp";

let value: Creator = {
  account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  value: 144494,
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      | Example                                                          |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `account`                                                        | *string*                                                         | :heavy_check_mark:                                               | Blockchain address in Union format `${blockchainGroup}:${token}` | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb              |
| `value`                                                          | *number*                                                         | :heavy_check_mark:                                               | N/A                                                              |                                                                  |