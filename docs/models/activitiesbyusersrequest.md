# ActivitiesByUsersRequest

## Example Usage

```typescript
import { ActivitiesByUsersRequest } from "@rarible/protocol-mcp";

let value: ActivitiesByUsersRequest = {
  types: [
    "SELL",
  ],
  users: [
    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  ],
  bidCurrencies: [
    "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
  ],
  blockchains: [
    "ETHEREUM",
  ],
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `types`                                                                                       | [models.UserActivityType](../models/useractivitytype.md)[]                                    | :heavy_check_mark:                                                                            | Activity type                                                                                 |
| `users`                                                                                       | *string*[]                                                                                    | :heavy_check_mark:                                                                            | List of the user id                                                                           |
| `bidCurrencies`                                                                               | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | Currency for BID and CANCEL_BID activity types                                                |
| `blockchains`                                                                                 | [models.Blockchain](../models/blockchain.md)[]                                                | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `from`                                                                                        | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | Lower time border of data                                                                     |
| `to`                                                                                          | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | Upper time border of data                                                                     |
| `continuation`                                                                                | *string*                                                                                      | :heavy_minus_sign:                                                                            | Continuation token from the previous response                                                 |
| `cursor`                                                                                      | *string*                                                                                      | :heavy_minus_sign:                                                                            | Combined continuation token from the previous response                                        |
| `size`                                                                                        | *number*                                                                                      | :heavy_minus_sign:                                                                            | The number of items to return                                                                 |
| `sort`                                                                                        | [models.ActivitySort](../models/activitysort.md)                                              | :heavy_minus_sign:                                                                            | Sorting by data update time                                                                   |