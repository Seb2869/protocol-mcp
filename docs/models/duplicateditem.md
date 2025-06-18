# DuplicatedItem

## Example Usage

```typescript
import { DuplicatedItem } from "@rarible/protocol-mcp";

let value: DuplicatedItem = {
  traitGroups: [
    {
      key: "Hat",
      value: "Halo",
    },
  ],
  count: 961586,
  item: {
    id:
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    blockchain: "ETHEREUM",
    collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    tokenId: "123456",
    creators: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 113311,
      },
    ],
    ownerIfSingle: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    lazySupply: "123456",
    pending: [
      {
        atType: "TRANSFER",
        from: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      },
    ],
    mintedAt: new Date("2023-05-25T16:29:10.539Z"),
    lastUpdatedAt: new Date("2023-04-20T20:57:09.218Z"),
    supply: "123456",
    meta: {
      name: "<value>",
      attributes: [
        {
          key: "<key>",
        },
      ],
      content: [
        {
          url: "https://sick-tectonics.net/",
          representation: "PORTRAIT",
          mimeType: "image/png",
        },
      ],
      extraContent: [
        {
          url: "https://pleasant-widow.net",
          representation: "INITIAL",
          mimeType: "image/png",
        },
      ],
    },
    deleted: false,
    bestSellOrder: {
      id:
        "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
      fill: "123456.789",
      platform: "OTHER",
      status: "FILLED",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2025-12-17T03:29:01.157Z"),
      lastUpdatedAt: new Date("2025-11-16T01:16:21.398Z"),
      makePrice: "123456.789",
      takePrice: "123456.789",
      makePriceUsd: "123456.789",
      takePriceUsd: "123456.789",
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      make: {
        type: {
          blockchain: "ETHEREUM",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          atType: "CURRENCY_NATIVE",
        },
        value: "123456.789",
      },
      take: {
        type: {
          atType: "ERC1155_Lazy",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
          tokenId: "123456",
          uri: "https://unknown-developing.org",
          supply: "123456",
          creators: [
            {
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 189992,
            },
          ],
          royalties: [
            {
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 724991,
            },
          ],
          signatures: [
            "<value>",
          ],
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
      platform: "VERSUM",
      status: "CANCELLED",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2024-06-15T18:11:45.295Z"),
      lastUpdatedAt: new Date("2025-12-30T05:54:29.995Z"),
      makePrice: "123456.789",
      takePrice: "123456.789",
      makePriceUsd: "123456.789",
      takePriceUsd: "123456.789",
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      make: {
        type: {
          atType: "CRYPTO_PUNKS",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
          tokenId: 84149,
        },
        value: "123456.789",
      },
      take: {
        type: {
          blockchain: "ETHEREUM",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          atType: "CURRENCY_NATIVE",
        },
        value: "123456.789",
      },
      salt: "<value>",
      feeTakers: [
        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      ],
      data: {
        atType: "ETH_OPEN_SEA_V1",
        exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        makerRelayerFee: "123456",
        takerRelayerFee: "123456",
        makerProtocolFee: "123456",
        takerProtocolFee: "123456",
        feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        feeMethod: "PROTOCOL_FEE",
        side: "SELL",
        saleKind: "FIXED_PRICE",
        howToCall: "DELEGATE_CALL",
        callData: "<value>",
        replacementPattern: "<value>",
        staticTarget: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        staticExtraData: "<value>",
        extra: "123456",
      },
    },
    bestBidOrdersByCurrency: [
      {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "OBJKT",
        status: "CANCELLED",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2025-03-09T19:36:10.745Z"),
        lastUpdatedAt: new Date("2025-03-04T03:53:55.115Z"),
        makePrice: "123456.789",
        takePrice: "123456.789",
        makePriceUsd: "123456.789",
        takePriceUsd: "123456.789",
        maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        make: {
          type: {
            atType: "ERC1155",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            tokenId: "123456",
          },
          value: "123456.789",
        },
        take: {
          type: {
            atType: "ERC20",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          },
          value: "123456.789",
        },
        salt: "<value>",
        feeTakers: [
          "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        ],
        data: {
          atType: "ETH_OPEN_SEA_V1",
          exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          makerRelayerFee: "123456",
          takerRelayerFee: "123456",
          makerProtocolFee: "123456",
          takerProtocolFee: "123456",
          feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          feeMethod: "SPLIT_FEE",
          side: "BUY",
          saleKind: "DUTCH_AUCTION",
          howToCall: "DELEGATE_CALL",
          callData: "<value>",
          replacementPattern: "<value>",
          staticTarget: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          staticExtraData: "<value>",
          extra: "123456",
        },
      },
    ],
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
          createdAt: new Date("2025-08-30T21:10:53.001Z"),
          lastUpdatedAt: new Date("2023-12-18T11:28:11.293Z"),
          makePrice: "123456.789",
          takePrice: "123456.789",
          makePriceUsd: "123456.789",
          takePriceUsd: "123456.789",
          maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          make: {
            type: {
              atType: "FLOW_FT",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            },
            value: "123456.789",
          },
          take: {
            type: {
              atType: "ETH",
              blockchain: "ETHEREUM",
            },
            value: "123456.789",
          },
          salt: "<value>",
          feeTakers: [
            "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          ],
          data: {
            atType: "IMMUTABLEX_RARIBLE_V1",
            payouts: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 744321,
              },
            ],
            originFees: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 47445,
              },
            ],
          },
        },
        bestBidOrder: {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "TEIA",
          status: "FILLED",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2025-02-10T20:09:58.061Z"),
          lastUpdatedAt: new Date("2024-07-01T23:14:54.884Z"),
          makePrice: "123456.789",
          takePrice: "123456.789",
          makePriceUsd: "123456.789",
          takePriceUsd: "123456.789",
          maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          make: {
            type: {
              atType: "ETH",
              blockchain: "ETHEREUM",
            },
            value: "123456.789",
          },
          take: {
            type: {
              atType: "ERC1155_Lazy",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
              tokenId: "123456",
              uri: "https://esteemed-vanadyl.org",
              supply: "123456",
              creators: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 717568,
                },
              ],
              royalties: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 701047,
                },
              ],
              signatures: [
                "<value>",
              ],
            },
            value: "123456.789",
          },
          salt: "<value>",
          feeTakers: [
            "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          ],
          data: {
            atType: "ETH_RARIBLE_V2_2",
            payouts: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 371107,
              },
            ],
            originFees: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 188596,
              },
            ],
            isMakeFill: false,
          },
        },
      },
    ],
    totalStock: "123456",
    sellers: 498344,
    lastSale: {
      date: new Date("2024-02-27T01:38:44.610Z"),
      seller: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: "123456.789",
      currency: {
        atType: "ERC20",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      },
      price: "123456.789",
    },
    itemCollection: {
      id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      name: "<value>",
      bestBidOrder: {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "RARIBLE",
        status: "FILLED",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2025-10-30T10:15:42.838Z"),
        lastUpdatedAt: new Date("2025-08-15T22:04:30.134Z"),
        makePrice: "123456.789",
        takePrice: "123456.789",
        makePriceUsd: "123456.789",
        takePriceUsd: "123456.789",
        maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        make: {
          type: {
            atType: "ERC721_Lazy",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            tokenId: "123456",
            uri: "https://blushing-finger.org/",
            creators: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 504961,
              },
            ],
            royalties: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 59758,
              },
            ],
            signatures: [
              "<value>",
            ],
          },
          value: "123456.789",
        },
        take: {
          type: {
            atType: "CRYPTO_PUNKS",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            tokenId: 123343,
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
          orderType: "PARTIAL_OPEN",
          offer: [
            {
              itemType: "ERC721",
              token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              identifierOrCriteria: "123456",
              startAmount: "123456",
              endAmount: "123456",
            },
          ],
          consideration: [
            {
              itemType: "NATIVE",
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
      bestSellOrder: {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "OPEN_SEA",
        status: "CANCELLED",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2023-03-17T17:39:14.544Z"),
        lastUpdatedAt: new Date("2025-03-21T00:55:57.308Z"),
        makePrice: "123456.789",
        takePrice: "123456.789",
        makePriceUsd: "123456.789",
        takePriceUsd: "123456.789",
        maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        make: {
          type: {
            atType: "NFT",
            collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            itemId:
              "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
          },
          value: "123456.789",
        },
        take: {
          type: {
            atType: "NFT_OF_COLLECTION",
            collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
          },
          value: "123456.789",
        },
        salt: "<value>",
        feeTakers: [
          "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        ],
        data: {
          atType: "ETH_OPEN_SEA_V1",
          exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          makerRelayerFee: "123456",
          takerRelayerFee: "123456",
          makerProtocolFee: "123456",
          takerProtocolFee: "123456",
          feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          feeMethod: "PROTOCOL_FEE",
          side: "SELL",
          saleKind: "DUTCH_AUCTION",
          howToCall: "DELEGATE_CALL",
          callData: "<value>",
          replacementPattern: "<value>",
          staticTarget: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          staticExtraData: "<value>",
          extra: "123456",
        },
      },
    },
  },
};
```

## Fields

| Field                                                        | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `traitGroups`                                                | [models.ItemTraitProperty](../models/itemtraitproperty.md)[] | :heavy_check_mark:                                           | N/A                                                          |
| `count`                                                      | *number*                                                     | :heavy_check_mark:                                           | Number of duplicated items in the group                      |
| `item`                                                       | [models.Item](../models/item.md)                             | :heavy_check_mark:                                           | N/A                                                          |