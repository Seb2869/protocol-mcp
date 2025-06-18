# LazyItemMintForm

## Example Usage

```typescript
import { LazyItemMintForm } from "@rarible/protocol-mcp";

let value: LazyItemMintForm = {
  item: {
    atType: "ETH_ERC1155",
    supply: "123456",
    id:
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    uri: "https://jagged-majority.info",
    creators: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 5552,
      },
    ],
    royalties: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 191246,
      },
    ],
    signatures: [
      "<value>",
    ],
  },
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `item`             | *models.LazyItem*  | :heavy_check_mark: | Type of an Asset   |