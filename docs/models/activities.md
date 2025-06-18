# Activities

## Example Usage

```typescript
import { Activities } from "@rarible/protocol-mcp";

let value: Activities = {
  activities: [
    {
      atType: "CANCEL_LIST",
      orderId:
        "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
      hash: "<value>",
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      make: {
        atType: "CURRENCY_TOKEN",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      },
      take: {
        atType: "ERC721",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        tokenId: "123456",
      },
      transactionHash: "<value>",
      id: "ETHEREUM:${id}",
      date: new Date("2025-08-27T22:52:50.259Z"),
    },
  ],
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `continuation`                                                   | *string*                                                         | :heavy_minus_sign:                                               | Continuation token to paginate activities search result          |
| `cursor`                                                         | *string*                                                         | :heavy_minus_sign:                                               | Combined continuation token to paginate activities search result |
| `activities`                                                     | *models.Activity*[]                                              | :heavy_check_mark:                                               | List of found activities                                         |