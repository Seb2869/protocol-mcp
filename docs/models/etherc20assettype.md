# EthErc20AssetType

## Example Usage

```typescript
import { EthErc20AssetType } from "@rarible/protocol-mcp";

let value: EthErc20AssetType = {
  atType: "ERC20",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            | Example                                                                |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `atType`                                                               | [models.EthErc20AssetTypeAtType](../models/etherc20assettypeattype.md) | :heavy_check_mark:                                                     | N/A                                                                    |                                                                        |
| `contract`                                                             | *string*                                                               | :heavy_check_mark:                                                     | Blockchain contract address in Union format `ETHEREUM:${token}`        | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                    |