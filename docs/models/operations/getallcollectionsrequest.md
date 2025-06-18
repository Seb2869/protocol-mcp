# GetAllCollectionsRequest

## Example Usage

```typescript
import { GetAllCollectionsRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetAllCollectionsRequest = {
  blockchains: [
    "ETHEREUM",
  ],
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `blockchains`                                                                                     | [models.Blockchain](../../models/blockchain.md)[]                                                 | :heavy_minus_sign:                                                                                | Names of the blockchain networks. If no one specified, data from all blockchains will be returned |
| `continuation`                                                                                    | *string*                                                                                          | :heavy_minus_sign:                                                                                | Continuation token from the previous response                                                     |
| `size`                                                                                            | *number*                                                                                          | :heavy_minus_sign:                                                                                | The number of items to return                                                                     |