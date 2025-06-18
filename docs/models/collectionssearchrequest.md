# CollectionsSearchRequest

Complex search request for collections

## Example Usage

```typescript
import { CollectionsSearchRequest } from "@rarible/protocol-mcp";

let value: CollectionsSearchRequest = {
  filter: {
    blockchains: [
      "ETHEREUM",
    ],
    text: "Apes",
  },
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `size`                                                                 | *number*                                                               | :heavy_minus_sign:                                                     | Number of entities returned                                            |
| `continuation`                                                         | *string*                                                               | :heavy_minus_sign:                                                     | Continuation token to paginate collections search result               |
| `filter`                                                               | [models.CollectionsSearchFilter](../models/collectionssearchfilter.md) | :heavy_check_mark:                                                     | Filter for collections search query                                    |