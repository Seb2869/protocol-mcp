# NativeCurrencyAssetType

## Example Usage

```typescript
import { NativeCurrencyAssetType } from "@rarible/protocol-mcp";

let value: NativeCurrencyAssetType = {
  blockchain: "ETHEREUM",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  atType: "CURRENCY_NATIVE",
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        | Example                                                                            |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `blockchain`                                                                       | [models.Blockchain](../models/blockchain.md)                                       | :heavy_check_mark:                                                                 | N/A                                                                                | ETHEREUM                                                                           |
| `contract`                                                                         | *string*                                                                           | :heavy_minus_sign:                                                                 | Blockchain contract address in Union format `ETHEREUM:${token}`                    | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                                |
| `atType`                                                                           | [models.NativeCurrencyAssetTypeAtType](../models/nativecurrencyassettypeattype.md) | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |