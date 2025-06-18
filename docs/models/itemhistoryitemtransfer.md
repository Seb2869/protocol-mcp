# ItemHistoryItemTransfer

## Example Usage

```typescript
import { ItemHistoryItemTransfer } from "@rarible/protocol-mcp";

let value: ItemHistoryItemTransfer = {
  atType: "TRANSFER",
  from: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  tokenId: "123456",
  value: "123456",
  date: new Date("2024-03-02T17:11:27.857Z"),
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `atType`                                                                                      | [models.ItemHistoryAtTypeTransfer](../models/itemhistoryattypetransfer.md)                    | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `from`                                                                                        | *string*                                                                                      | :heavy_check_mark:                                                                            | Blockchain address in Union format `${blockchainGroup}:${token}`                              | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                           |
| `owner`                                                                                       | *string*                                                                                      | :heavy_check_mark:                                                                            | Blockchain address in Union format `${blockchainGroup}:${token}`                              | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                           |
| `contract`                                                                                    | *string*                                                                                      | :heavy_check_mark:                                                                            | Blockchain contract address in Union format `ETHEREUM:${token}`                               | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                                           |
| `tokenId`                                                                                     | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           | 123456                                                                                        |
| `value`                                                                                       | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           | 123456                                                                                        |
| `date`                                                                                        | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |