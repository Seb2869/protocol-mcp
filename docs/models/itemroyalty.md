# ItemRoyalty

## Example Usage

```typescript
import { ItemRoyalty } from "@rarible/protocol-mcp";

let value: ItemRoyalty = {
  atType: "ROYALTY",
  royalties: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 979636,
    },
  ],
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  tokenId: "123456",
  value: "123456",
  date: new Date("2025-07-21T08:09:13.919Z"),
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `atType`                                                                                      | [models.AtTypeRoyalty](../models/attyperoyalty.md)                                            | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `royalties`                                                                                   | [models.Royalty](../models/royalty.md)[]                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `owner`                                                                                       | *string*                                                                                      | :heavy_minus_sign:                                                                            | Blockchain address in Union format `${blockchainGroup}:${token}`                              | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                           |
| `contract`                                                                                    | *string*                                                                                      | :heavy_check_mark:                                                                            | Blockchain contract address in Union format `ETHEREUM:${token}`                               | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                                           |
| `tokenId`                                                                                     | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           | 123456                                                                                        |
| `value`                                                                                       | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           | 123456                                                                                        |
| `date`                                                                                        | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |