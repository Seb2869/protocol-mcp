# ItemWithOwnership

## Example Usage

```typescript
import { ItemWithOwnership } from "@rarible/protocol-mcp";

let value: ItemWithOwnership = {
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
        value: 950890,
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
    mintedAt: new Date("2023-05-03T22:24:00.313Z"),
    lastUpdatedAt: new Date("2023-12-22T08:41:59.897Z"),
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
          url: "https://fake-governance.biz/",
          representation: "BIG",
          mimeType: "image/png",
        },
      ],
      extraContent: [
        {
          url: "https://bony-pantyhose.org",
          representation: "BIG",
          mimeType: "image/png",
        },
      ],
    },
    deleted: false,
    bestSellOrder: {
      id:
        "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
      fill: "123456.789",
      platform: "OBJKT",
      status: "ACTIVE",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2023-09-20T17:37:37.515Z"),
      lastUpdatedAt: new Date("2024-01-09T17:14:01.691Z"),
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
          uri: "https://salty-papa.net/",
          creators: [
            {
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 829214,
            },
          ],
          royalties: [
            {
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 102095,
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
          atType: "ERC721",
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
        orderType: "PARTIAL_OPEN",
        offer: [
          {
            itemType: "NATIVE",
            token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            identifierOrCriteria: "123456",
            startAmount: "123456",
            endAmount: "123456",
          },
        ],
        consideration: [
          {
            itemType: "ERC721",
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
    bestBidOrder: {
      id:
        "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
      fill: "123456.789",
      platform: "TEIA",
      status: "ACTIVE",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2024-02-13T06:08:25.347Z"),
      lastUpdatedAt: new Date("2024-03-22T04:56:06.183Z"),
      makePrice: "123456.789",
      takePrice: "123456.789",
      makePriceUsd: "123456.789",
      takePriceUsd: "123456.789",
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      make: {
        type: {
          atType: "COLLECTION",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        },
        value: "123456.789",
      },
      take: {
        type: {
          atType: "NFT",
          collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
          itemId:
            "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
        },
        value: "123456.789",
      },
      salt: "<value>",
      feeTakers: [
        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      ],
      data: {
        atType: "ETH_RARIBLE_V1",
        fee: "123456",
      },
    },
    bestBidOrdersByCurrency: [
      {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "TEIA",
        status: "ACTIVE",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2025-06-01T06:56:44.189Z"),
        lastUpdatedAt: new Date("2025-05-05T21:08:20.609Z"),
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
            atType: "FLOW_FT",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
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
    ],
    originOrders: [
      {
        origin: "<value>",
        bestSellOrder: {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "FXHASH",
          status: "INACTIVE",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2023-10-29T08:39:51.987Z"),
          lastUpdatedAt: new Date("2024-06-21T19:43:10.006Z"),
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
              atType: "ERC721",
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
            atType: "ETH_CRYPTO_PUNKS",
            stub: "STUB",
          },
        },
        bestBidOrder: {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "CRYPTO_PUNKS",
          status: "FILLED",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2025-01-30T17:16:58.177Z"),
          lastUpdatedAt: new Date("2025-01-31T21:01:12.404Z"),
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
            atType: "ETH_OPEN_SEA_V1",
            exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            makerRelayerFee: "123456",
            takerRelayerFee: "123456",
            makerProtocolFee: "123456",
            takerProtocolFee: "123456",
            feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            feeMethod: "PROTOCOL_FEE",
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
      },
    ],
    totalStock: "123456",
    sellers: 353096,
    lastSale: {
      date: new Date("2025-08-09T01:23:26.025Z"),
      seller: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: "123456.789",
      currency: {
        atType: "CURRENCY_TOKEN",
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
        status: "INACTIVE",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2023-06-23T10:33:20.570Z"),
        lastUpdatedAt: new Date("2024-03-18T06:45:30.615Z"),
        makePrice: "123456.789",
        takePrice: "123456.789",
        makePriceUsd: "123456.789",
        takePriceUsd: "123456.789",
        maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        make: {
          type: {
            atType: "SOLANA_NFT",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            itemId:
              "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
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
          atType: "ETH_BASIC_SEAPORT_DATA_V1",
          protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          orderType: "PARTIAL_RESTRICTED",
          offer: [
            {
              itemType: "ERC20",
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
        platform: "FXHASH",
        status: "INACTIVE",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2023-08-16T11:15:21.487Z"),
        lastUpdatedAt: new Date("2025-12-28T22:57:21.573Z"),
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
            tokenId: 751539,
          },
          value: "123456.789",
        },
        take: {
          type: {
            atType: "ERC1155",
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
          atType: "ETH_OPEN_SEA_V1",
          exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          makerRelayerFee: "123456",
          takerRelayerFee: "123456",
          makerProtocolFee: "123456",
          takerProtocolFee: "123456",
          feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          feeMethod: "PROTOCOL_FEE",
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
    },
  },
  ownership: {
    id:
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410:0x4765273c477c2dc484da4f1984639e943adccfeb",
    blockchain: "ETHEREUM",
    collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: "123456",
    createdAt: new Date("2024-02-24T19:00:27.774Z"),
    creators: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 13181,
      },
    ],
    lazyValue: "123456",
  },
};
```

## Fields

| Field                                              | Type                                               | Required                                           | Description                                        |
| -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- |
| `item`                                             | [models.Item](../models/item.md)                   | :heavy_check_mark:                                 | N/A                                                |
| `ownership`                                        | [models.ItemOwnership](../models/itemownership.md) | :heavy_check_mark:                                 | N/A                                                |