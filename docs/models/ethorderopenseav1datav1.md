# EthOrderOpenSeaV1DataV1

## Example Usage

```typescript
import { EthOrderOpenSeaV1DataV1 } from "@rarible/protocol-mcp";

let value: EthOrderOpenSeaV1DataV1 = {
  atType: "ETH_OPEN_SEA_V1",
  exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  makerRelayerFee: "123456",
  takerRelayerFee: "123456",
  makerProtocolFee: "123456",
  takerProtocolFee: "123456",
  feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  feeMethod: "PROTOCOL_FEE",
  side: "SELL",
  saleKind: "FIXED_PRICE",
  howToCall: "DELEGATE_CALL",
  callData: "<value>",
  replacementPattern: "<value>",
  staticTarget: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  staticExtraData: "<value>",
  extra: "123456",
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        | Example                                                                            |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `atType`                                                                           | [models.EthOrderOpenSeaV1DataV1AtType](../models/ethorderopenseav1datav1attype.md) | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `exchange`                                                                         | *string*                                                                           | :heavy_check_mark:                                                                 | Blockchain address in Union format `${blockchainGroup}:${token}`                   | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                |
| `makerRelayerFee`                                                                  | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                | 123456                                                                             |
| `takerRelayerFee`                                                                  | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                | 123456                                                                             |
| `makerProtocolFee`                                                                 | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                | 123456                                                                             |
| `takerProtocolFee`                                                                 | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                | 123456                                                                             |
| `feeRecipient`                                                                     | *string*                                                                           | :heavy_check_mark:                                                                 | Blockchain address in Union format `${blockchainGroup}:${token}`                   | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                |
| `feeMethod`                                                                        | [models.FeeMethod](../models/feemethod.md)                                         | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `side`                                                                             | [models.Side](../models/side.md)                                                   | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `saleKind`                                                                         | [models.SaleKind](../models/salekind.md)                                           | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `howToCall`                                                                        | [models.HowToCall](../models/howtocall.md)                                         | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `callData`                                                                         | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `replacementPattern`                                                               | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `staticTarget`                                                                     | *string*                                                                           | :heavy_check_mark:                                                                 | Blockchain address in Union format `${blockchainGroup}:${token}`                   | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                |
| `staticExtraData`                                                                  | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `extra`                                                                            | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                | 123456                                                                             |