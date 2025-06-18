# EthSeaportOffer

## Example Usage

```typescript
import { EthSeaportOffer } from "@rarible/protocol-mcp";

let value: EthSeaportOffer = {
  itemType: "ERC1155_WITH_CRITERIA",
  token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  identifierOrCriteria: "123456",
  startAmount: "123456",
  endAmount: "123456",
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      | Example                                                          |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `itemType`                                                       | [models.EthSeaportItemType](../models/ethseaportitemtype.md)     | :heavy_check_mark:                                               | N/A                                                              |                                                                  |
| `token`                                                          | *string*                                                         | :heavy_check_mark:                                               | Blockchain address in Union format `${blockchainGroup}:${token}` | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb              |
| `identifierOrCriteria`                                           | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              | 123456                                                           |
| `startAmount`                                                    | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              | 123456                                                           |
| `endAmount`                                                      | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              | 123456                                                           |