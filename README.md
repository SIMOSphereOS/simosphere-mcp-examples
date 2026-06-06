[![smithery badge](https://smithery.ai/badge/simosphereai/simosphere-ai)](https://smithery.ai/servers/simosphereai/simosphere-ai)

# SIMOSphere AI MCP Examples

Model Context Protocol (MCP) integration examples for [SIMOSphere AI](https://simosphereai.com).

Connect enterprise data sources (CRM, ERP, SharePoint, DMS) with AI agents — GDPR-compliant, EU-hosted.

## MCP Server

- **URL**: https://mcp.simosphereai.com
- **Transport**: Streamable HTTP
- **Auth**: Bearer token (API key)
- **Server Card**: https://simosphereai.com/.well-known/mcp/server-card.json
- **Manifest**: https://simosphereai.com/.well-known/mcp/manifest.json

## Available Tools

| Tool | Description |
|------|-------------|
| `search_documents` | Search SharePoint, DMS, local files |
| `query_database` | Read-only queries against Dynamics 365, ERP, CRM |
| `create_record` | Create records in CRM/ERP systems |
| `send_notification` | Send via email, Teams, or Slack |

## Claude Desktop Config

```json
{
  "mcpServers": {
    "simosphere": {
      "command": "npx",
      "args": ["-y", "@simosphere/mcp-client"],
      "env": {
        "SIMOSPHERE_API_KEY": "sk-simo-your-key-here"
      }
    }
  }
}
```

## Cursor / VS Code Config

Add to MCP settings:
- Server URL: `https://mcp.simosphereai.com`
- Auth: Bearer `sk-simo-your-key-here`

## Azure Marketplace

SIMOSphere M365 Governance is available on the [Microsoft Azure Marketplace](https://marketplace.microsoft.com/en-us/product/azure-application/simosimplemarketing1619635742390.simosphere-m365-governance-preview).

## Resources

- **Docs**: https://simosphereai.com/de/developers
- **MCP Spec**: https://simosphereai.com/de/mcp-server
- **API**: https://api.simosphereai.com/openapi.json
- **SDK**: https://www.npmjs.com/package/@simosphere/sdk

Engineered at SIMO GmbH · Aschaffenburg, Germany
