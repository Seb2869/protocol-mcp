# OlapOwnerStatistic

## Example Usage

```typescript
import { OlapOwnerStatistic } from "@rarible/protocol-mcp";

let value: OlapOwnerStatistic = {
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  ownedItems: 252558,
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      | Example                                                          |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `owner`                                                          | *string*                                                         | :heavy_check_mark:                                               | Blockchain address in Union format `${blockchainGroup}:${token}` | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb              |
| `ownedItems`                                                     | *number*                                                         | :heavy_check_mark:                                               | N/A                                                              |                                                                  |