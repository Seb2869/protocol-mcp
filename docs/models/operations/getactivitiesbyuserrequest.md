# GetActivitiesByUserRequest

## Example Usage

```typescript
import { GetActivitiesByUserRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetActivitiesByUserRequest = {
  type: [
    "MINT",
  ],
  blockchains: [
    "ETHEREUM",
  ],
  user: [
    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  ],
  bidCurrencies: [
    "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
  ],
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `type`                                                                                        | [models.UserActivityType](../../models/useractivitytype.md)[]                                 | :heavy_check_mark:                                                                            | Activity type                                                                                 |
| `blockchains`                                                                                 | [models.Blockchain](../../models/blockchain.md)[]                                             | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `user`                                                                                        | *string*[]                                                                                    | :heavy_check_mark:                                                                            | Addresses of the users                                                                        |
| `bidCurrencies`                                                                               | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | Currency for BID and CANCEL_BID activity types                                                |
| `from`                                                                                        | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | Lower time border of data                                                                     |
| `to`                                                                                          | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | Upper time border of data                                                                     |
| `continuation`                                                                                | *string*                                                                                      | :heavy_minus_sign:                                                                            | Continuation token from the previous response                                                 |
| `cursor`                                                                                      | *string*                                                                                      | :heavy_minus_sign:                                                                            | Combined continuation token from the previous response                                        |
| `size`                                                                                        | *number*                                                                                      | :heavy_minus_sign:                                                                            | The number of items to return                                                                 |
| `sort`                                                                                        | [models.ActivitySort](../../models/activitysort.md)                                           | :heavy_minus_sign:                                                                            | Sorting by data update time                                                                   |