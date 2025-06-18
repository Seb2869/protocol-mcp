# QueryTraitsRequest

## Example Usage

```typescript
import { QueryTraitsRequest } from "@rarible/protocol-mcp/models/operations";

let value: QueryTraitsRequest = {
  keys: [
    "Hat",
  ],
  collectionIds: [
    "ETHEREUM:0x60e4d786628fea6478f785a6d7e704777c86a7c6",
  ],
  owners: [
    "${filterOwners}",
  ],
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `keys`                                                                           | *string*[]                                                                       | :heavy_minus_sign:                                                               | Trait keys for strict filtering (if not specified - all traits will be returned) |
| `collectionIds`                                                                  | *string*[]                                                                       | :heavy_check_mark:                                                               | Collections identifiers to which traits belong                                   |
| `owners`                                                                         | *string*[]                                                                       | :heavy_minus_sign:                                                               | Return traits only for items owned by user                                       |