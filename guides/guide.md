# 📖 Guide to Using @rarible/protocol-mcp

This guide covers three key ways to get started with the `@rarible/protocol-mcp` SDK: integrating with Claude, integrating with ChatGPT, self-hosting the MCP server, and leveraging the OpenAPI specification for custom integrations.

## Prerequisites
- **Node.js**: Version 20 or higher.
- **Rarible API Key**: Obtain from [https://rarible.org/pricing](https://rarible.org/pricing).
- **Environment Setup**: Set the API key as an environment variable:
  ```bash
  export RARIBLE_API_KEY="your-api-key-here"
  ```
- **Tools**: Familiarity with TypeScript/JavaScript, terminal commands, and optionally Postman or OpenAPI Generator.

## Quick Start: Claude Integration
Integrate the SDK with Claude/OpenAI to enable AI-driven interactions using the MCP server.

### Installation
Install the SDK:
```bash
npm install @rarible/protocol-mcp
```
Or use `pnpm`, `bun`, or `yarn`:
```bash
pnpm add @rarible/protocol-mcp
bun add @rarible/protocol-mcp
yarn add @rarible/protocol-mcp zod
```

### Configure Claude
1. **Update Config**:
   Add the MCP server to `claude_desktop_config.json`:
   ```json
   {
     "mcpServers": {
       "RaribleProtocolMcp": {
         "command": "npx",
         "args": [
           "-y", "--package", "@rarible/protocol-mcp",
           "--",
           "mcp", "start",
           "--api-key-auth", "your-api-key-here"
         ]
       }
     }
   }
   ```
2. **Restart Claude**

### Usage
- In Claude, use queries like "Fetch NFT details for ID ETHEREUM:0x..." or "Get collection floor price."
- Claude maps these to SDK methods (e.g., `nftItems.getItemById`) and returns formatted results.

### Troubleshooting
- Verify API key and Node.js version (`node -v`).
- Check Claude logs for errors like `UnionApiErrorBadRequest`.

## ChatGPT Integration
Integrate the SDK with ChatGPT using OpenAI's MCP support to enable AI-driven interactions.

### Prerequisites
- **OpenAI API Key**: Obtain from [https://platform.openai.com/api-keys](https://platform.openai.com/api-keys)
- **MCP Server**: A publicly accessible MCP server endpoint (see Self-Hosting section below)
- **Rarible API Key**: Set on your MCP server

### Setup
1. **Deploy MCP Server**: Ensure your MCP server is running and accessible via HTTPS
2. **Configure ChatGPT**: Use the OpenAI API with MCP tools configuration

### Usage Example
Use the OpenAI API with MCP tools to interact with Rarible Protocol:

```bash
curl https://api.openai.com/v1/responses \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_OPENAI_API_KEY" \
  -d '{
    "model": "o4-mini-2025-04-16",
    "tools": [
      {
        "type": "mcp",
        "server_label": "rarible-protocol",
        "server_url": "https://your-mcp-server.com/sse",
        "require_approval": "never"
      }
    ],
    "input": "please find NFT tokens for the owner ETHEREUM:0x28e0A9154Ed24988f30B743b5F3Cf060CC4234C0"
  }'
```

### Configuration Parameters
- **`model`**: Use compatible OpenAI models (e.g., `o4-mini-2025-04-16`)
- **`server_label`**: Identifier for your MCP server
- **`server_url`**: Public HTTPS endpoint of your MCP server
- **`require_approval`**: Set to `"never"` for automatic tool execution

### Common Use Cases
- **NFT Discovery**: "Find NFTs owned by address ETHEREUM:0x..."
- **Collection Analysis**: "Get floor price for collection X"
- **Market Data**: "Show recent sales for NFT Y"
- **Ownership Queries**: "List all collections owned by address Z"

### Troubleshooting
- **401 Unauthorized**: Verify your OpenAI API key
- **MCP Server Errors**: Ensure your server is publicly accessible and HTTPS-enabled
- **Rate Limits**: Handle OpenAI API rate limits according to your plan
- **Tool Execution**: Check MCP server logs for Rarible API errors

## Self-Hosting Quick Start
Run the SDK as a local or cloud-hosted MCP server for direct API access.

### Installation
1. **Create Project**:
   ```bash
   mkdir rarible-mcp-server
   cd rarible-mcp-server
   npm init -y
   npm install @rarible/protocol-mcp
   ```

2. **Start Server**:
   ```bash
   npx -y --package @rarible/protocol-mcp -- mcp start --api-key-auth $RARIBLE_API_KEY --protocol sse
   ```

3. **Optional: Customize**:
   Change port or add options:
   ```bash
   npx -y --package @rarible/protocol-mcp -- mcp start --api-key-auth $RARIBLE_API_KEY --port 8080 --protocol sse
   ```

### Test the Server
- Run MCP server locally
   ```bash
   npx -y --package @rarible/protocol-mcp -- mcp start --api-key-auth $RARIBLE_API_KEY --port 8080 --protocol sse
   ```
- Run MCP inspector:
  ```bash
  npx @modelcontextprotocol/inspector
  ```
- Connect to mcp server an run tools:


### SDK Integration
1. **Install SDK**:
   ```bash
   npm install @rarible/protocol-mcp
   ```
2. **Example Usage**:
   ```typescript
   import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

   const sdk = new RaribleProtocolMcp({
     apiKeyAuth: process.env.RARIBLE_API_KEY || "your-api-key-here",
   });

   async function run() {
     const result = await sdk.nftItems.getItemById({
       itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
     });
     console.log(result);
   }
   run();
   ```

### Custom HTTP Client
- Customize requests:
  ```typescript
  import { HTTPClient } from "@rarible/protocol-mcp/lib/http";

  const httpClient = new HTTPClient({ fetcher: fetch });
  httpClient.addHook("beforeRequest", (request) => {
    request.headers.set("x-custom-header", "custom-value");
    return request;
  });

  const sdk = new RaribleProtocolMcp({ httpClient, apiKeyAuth: "your-api-key-here" });
  ```

### Troubleshooting
- Verify API key permissions and spec version.
- Handle rate limits (`429` errors) per Rarible's documentation.

## Next Steps
- Explore [Rarible Protocol documentation](https://rarible.org) for advanced features.

