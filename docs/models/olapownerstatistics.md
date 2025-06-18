# OlapOwnerStatistics

## Example Usage

```typescript
import { OlapOwnerStatistics } from "@rarible/protocol-mcp";

let value: OlapOwnerStatistics = {
  owners: [
    {
      owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      ownedItems: 222705,
    },
  ],
};
```

## Fields

| Field                                                          | Type                                                           | Required                                                       | Description                                                    |
| -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
| `owners`                                                       | [models.OlapOwnerStatistic](../models/olapownerstatistic.md)[] | :heavy_check_mark:                                             | N/A                                                            |
| `continuation`                                                 | *string*                                                       | :heavy_minus_sign:                                             | Continuation token to paginate result                          |