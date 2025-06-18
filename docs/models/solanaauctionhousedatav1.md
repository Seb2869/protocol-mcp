# SolanaAuctionHouseDataV1

## Example Usage

```typescript
import { SolanaAuctionHouseDataV1 } from "@rarible/protocol-mcp";

let value: SolanaAuctionHouseDataV1 = {
  atType: "SOLANA_AUCTION_HOUSE_V1",
  auctionHouse: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

## Fields

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          | Example                                                                              |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `atType`                                                                             | [models.SolanaAuctionHouseDataV1AtType](../models/solanaauctionhousedatav1attype.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |                                                                                      |
| `fee`                                                                                | *number*                                                                             | :heavy_minus_sign:                                                                   | N/A                                                                                  |                                                                                      |
| `requiresSignOff`                                                                    | *boolean*                                                                            | :heavy_minus_sign:                                                                   | N/A                                                                                  |                                                                                      |
| `auctionHouse`                                                                       | *string*                                                                             | :heavy_minus_sign:                                                                   | Blockchain contract address in Union format `ETHEREUM:${token}`                      | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                                  |