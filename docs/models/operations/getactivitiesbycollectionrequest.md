# GetActivitiesByCollectionRequest

## Example Usage

```typescript
import { GetActivitiesByCollectionRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetActivitiesByCollectionRequest = {
  type: [
    "BID",
  ],
  collection: [
    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  ],
  bidCurrencies: [
    "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
  ],
};
```

## Fields

| Field                                                  | Type                                                   | Required                                               | Description                                            |
| ------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------ |
| `type`                                                 | [models.ActivityType](../../models/activitytype.md)[]  | :heavy_check_mark:                                     | Activity type                                          |
| `collection`                                           | *string*[]                                             | :heavy_check_mark:                                     | Address of the collection                              |
| `bidCurrencies`                                        | *string*[]                                             | :heavy_minus_sign:                                     | Currency for BID and CANCEL_BID activity types         |
| `continuation`                                         | *string*                                               | :heavy_minus_sign:                                     | Continuation token from the previous response          |
| `cursor`                                               | *string*                                               | :heavy_minus_sign:                                     | Combined continuation token from the previous response |
| `size`                                                 | *number*                                               | :heavy_minus_sign:                                     | The number of items to return                          |
| `sort`                                                 | [models.ActivitySort](../../models/activitysort.md)    | :heavy_minus_sign:                                     | Sorting by data update time                            |