# Ownerships

## Example Usage

```typescript
import { Ownerships } from "@rarible/protocol-mcp";

let value: Ownerships = {
  ownerships: [
    {
      id:
        "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410:0x4765273c477c2dc484da4f1984639e943adccfeb",
      blockchain: "ETHEREUM",
      itemId:
        "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      tokenId: "123456",
      owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: "123456",
      createdAt: new Date("2023-10-15T11:48:26.629Z"),
      lazyValue: "123456",
      pending: [
        {
          atType: "ROYALTY",
          royalties: [
            {
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 222939,
            },
          ],
          owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          tokenId: "123456",
          value: "123456",
          date: new Date("2024-10-26T07:11:52.884Z"),
        },
      ],
      bestSellOrder: {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "OPEN_SEA",
        status: "FILLED",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2023-04-17T12:09:24.616Z"),
        lastUpdatedAt: new Date("2025-10-19T18:37:05.725Z"),
        makePrice: "123456.789",
        takePrice: "123456.789",
        makePriceUsd: "123456.789",
        takePriceUsd: "123456.789",
        maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        make: {
          type: {
            atType: "GEN_ART",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
          },
          value: "123456.789",
        },
        take: {
          type: {
            atType: "FLOW_NFT",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            tokenId: "123456",
          },
          value: "123456.789",
        },
        salt: "<value>",
        feeTakers: [
          "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        ],
        data: {
          atType: "ETH_BASIC_SEAPORT_DATA_V1",
          protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          orderType: "CONTRACT",
          offer: [
            {
              itemType: "ERC721_WITH_CRITERIA",
              token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              identifierOrCriteria: "123456",
              startAmount: "123456",
              endAmount: "123456",
            },
          ],
          consideration: [
            {
              itemType: "ERC20",
              token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              identifierOrCriteria: "123456",
              startAmount: "123456",
              endAmount: "123456",
              recipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            },
          ],
          zone: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          zoneHash: "<value>",
          conduitKey: "<value>",
          nonce: "123456",
        },
      },
      originOrders: [
        {
          origin: "<value>",
          bestSellOrder: {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "OTHER",
            status: "INACTIVE",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2023-01-16T16:37:47.475Z"),
            lastUpdatedAt: new Date("2023-08-19T17:07:44.124Z"),
            makePrice: "123456.789",
            takePrice: "123456.789",
            makePriceUsd: "123456.789",
            takePriceUsd: "123456.789",
            maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            make: {
              type: {
                atType: "CURRENCY_TOKEN",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              },
              value: "123456.789",
            },
            take: {
              type: {
                atType: "ERC721",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                collection:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                tokenId: "123456",
              },
              value: "123456.789",
            },
            salt: "<value>",
            feeTakers: [
              "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            ],
            data: {
              atType: "RAW",
            },
          },
          bestBidOrder: {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "HEN",
            status: "CANCELLED",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2024-08-21T05:45:50.561Z"),
            lastUpdatedAt: new Date("2024-12-01T18:21:23.744Z"),
            makePrice: "123456.789",
            takePrice: "123456.789",
            makePriceUsd: "123456.789",
            takePriceUsd: "123456.789",
            maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            make: {
              type: {
                atType: "SOLANA_SOL",
              },
              value: "123456.789",
            },
            take: {
              type: {
                atType: "CURRENCY_TOKEN",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              },
              value: "123456.789",
            },
            salt: "<value>",
            feeTakers: [
              "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            ],
            data: {
              atType: "ETH_RARIBLE_V2_DATA_V3_BUY",
              payout: {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 366798,
              },
              originFeeFirst: {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 500052,
              },
              originFeeSecond: {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 924257,
              },
            },
          },
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                                               | Type                                                                                                                                                                | Required                                                                                                                                                            | Description                                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ~~`total`~~                                                                                                                                                         | *number*                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                  | : warning: ** DEPRECATED **: This will be removed in a future release, please migrate away from it as soon as possible.<br/><br/>Number of ownerships were found by request |
| `continuation`                                                                                                                                                      | *string*                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                  | Continuation token to paginate Ownerships search result                                                                                                             |
| `ownerships`                                                                                                                                                        | [models.Ownership](../models/ownership.md)[]                                                                                                                        | :heavy_check_mark:                                                                                                                                                  | List of found ownerships                                                                                                                                            |