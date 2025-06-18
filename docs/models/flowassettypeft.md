# FlowAssetTypeFt

## Example Usage

```typescript
import { FlowAssetTypeFt } from "@rarible/protocol-mcp";

let value: FlowAssetTypeFt = {
  atType: "FLOW_FT",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

## Fields

| Field                                                              | Type                                                               | Required                                                           | Description                                                        | Example                                                            |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `atType`                                                           | [models.FlowAssetTypeFtAtType](../models/flowassettypeftattype.md) | :heavy_check_mark:                                                 | N/A                                                                |                                                                    |
| `contract`                                                         | *string*                                                           | :heavy_check_mark:                                                 | Blockchain contract address in Union format `ETHEREUM:${token}`    | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                |