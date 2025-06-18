# GetOwnershipsByCollectionRequest

## Example Usage

```typescript
import { GetOwnershipsByCollectionRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetOwnershipsByCollectionRequest = {
  collection: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         | Example                                             |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `collection`                                        | *string*                                            | :heavy_check_mark:                                  | Address of the collection                           | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430 |
| `continuation`                                      | *string*                                            | :heavy_minus_sign:                                  | Continuation token from the previous response       |                                                     |
| `size`                                              | *number*                                            | :heavy_minus_sign:                                  | The number of items to return                       |                                                     |