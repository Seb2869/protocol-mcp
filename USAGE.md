<!-- Start SDK Example Usage [usage] -->
```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLEPROTOCOLMCP_API_KEY_AUTH"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftItems.getItemById({
    itemId:
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  });

  // Handle the result
  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->