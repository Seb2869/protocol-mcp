# GenerateTokenIdRequest

## Example Usage

```typescript
import { GenerateTokenIdRequest } from "@rarible/protocol-mcp/models/operations";

let value: GenerateTokenIdRequest = {
  collection: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  minter: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         | Example                                             |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `collection`                                        | *string*                                            | :heavy_check_mark:                                  | Address of the NFT collection                       | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430 |
| `minter`                                            | *string*                                            | :heavy_check_mark:                                  | Minter address                                      | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb |