# SolanaFtAssetType

## Example Usage

```typescript
import { SolanaFtAssetType } from "@rarible/protocol-mcp";

let value: SolanaFtAssetType = {
  atType: "SOLANA_FT",
  address: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            | Example                                                                |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `atType`                                                               | [models.SolanaFtAssetTypeAtType](../models/solanaftassettypeattype.md) | :heavy_check_mark:                                                     | N/A                                                                    |                                                                        |
| `address`                                                              | *string*                                                               | :heavy_check_mark:                                                     | Blockchain contract address in Union format `ETHEREUM:${token}`        | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                    |