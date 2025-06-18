# EthOrderBasicSeaportDataV1

## Example Usage

```typescript
import { EthOrderBasicSeaportDataV1 } from "@rarible/protocol-mcp";

let value: EthOrderBasicSeaportDataV1 = {
  atType: "ETH_BASIC_SEAPORT_DATA_V1",
  protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  orderType: "PARTIAL_OPEN",
  offer: [
    {
      itemType: "ERC20",
      token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      identifierOrCriteria: "123456",
      startAmount: "123456",
      endAmount: "123456",
    },
  ],
  consideration: [
    {
      itemType: "ERC1155",
      token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      identifierOrCriteria: "123456",
      startAmount: "123456",
      endAmount: "123456",
      recipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    },
  ],
  zone: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  zoneHash: "<value>",
  conduitKey: "<value>",
  nonce: "123456",
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             | Example                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `atType`                                                                                                                | [models.EthOrderSeaportDataV1AtType](../models/ethorderseaportdatav1attype.md)                                          | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `protocol`                                                                                                              | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | Blockchain address in Union format `${blockchainGroup}:${token}`                                                        | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                                                     |
| `orderType`                                                                                                             | [models.EthSeaportOrderType](../models/ethseaportordertype.md)                                                          | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `offer`                                                                                                                 | [models.EthSeaportOffer](../models/ethseaportoffer.md)[]                                                                | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `consideration`                                                                                                         | [models.EthSeaportConsideration](../models/ethseaportconsideration.md)[]                                                | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `zone`                                                                                                                  | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | Blockchain address in Union format `${blockchainGroup}:${token}`                                                        | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                                                     |
| `zoneHash`                                                                                                              | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `conduitKey`                                                                                                            | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| ~~`counter`~~                                                                                                           | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | : warning: ** DEPRECATED **: This will be removed in a future release, please migrate away from it as soon as possible. |                                                                                                                         |
| `nonce`                                                                                                                 | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     | 123456                                                                                                                  |