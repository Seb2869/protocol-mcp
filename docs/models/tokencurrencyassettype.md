# TokenCurrencyAssetType

## Example Usage

```typescript
import { TokenCurrencyAssetType } from "@rarible/protocol-mcp";

let value: TokenCurrencyAssetType = {
  atType: "CURRENCY_TOKEN",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      | Example                                                                          |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `atType`                                                                         | [models.TokenCurrencyAssetTypeAtType](../models/tokencurrencyassettypeattype.md) | :heavy_check_mark:                                                               | N/A                                                                              |                                                                                  |
| `contract`                                                                       | *string*                                                                         | :heavy_check_mark:                                                               | Blockchain contract address in Union format `ETHEREUM:${token}`                  | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                              |