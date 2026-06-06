# AGENTS.md — SIMOSphere AI MCP Examples

## Project
SIMOSphere AI — European AI orchestration platform for enterprises.
MCP server + OpenAI-compatible REST API, hosted in Germany (EU data residency).

## Main APIs
- REST API: https://api.simosphereai.com (OpenAPI: https://api.simosphereai.com/openapi.json)
- MCP Server: https://simosphereai.com/.well-known/mcp (Streamable HTTP)

## Authentication
- API Key: Bearer token in Authorization header
- Get a key: https://onboarding.simosphereai.com/register

## MCP Server
- URL: https://simosphereai.com/.well-known/mcp
- Transport: Streamable HTTP
- Auth: Bearer sk-simo-... token

## MCP Tools
- search_documents, query_database, create_record, send_notification

## SDKs
- npm: @simosphere/sdk, @simosphere/cli, @simosphere/mcp-server

## Quick Start (OpenAI-compatible)
```typescript
import OpenAI from "openai";
const client = new OpenAI({
  baseURL: "https://api.simosphereai.com/v1",
  apiKey: process.env.SIMO_API_KEY,
});
```

## Quick Start (MCP)
```json
{
  "mcpServers": {
    "simosphere": {
      "url": "https://simosphereai.com/.well-known/mcp",
      "headers": { "Authorization": "Bearer sk-simo-..." }
    }
  }
}
```

## CLI
```bash
npm install -g @simosphere/cli
simosphere health
simosphere models
simosphere chat "Hello"
```

## Data Residency
EU only (Germany). GDPR-compliant. EU AI Act-ready.

## Resources
- Developer docs: https://simosphereai.com/en/docs
- llms.txt: https://simosphereai.com/llms.txt
- llms-full.txt: https://onboarding.simosphereai.com/llms-full.txt
- OpenAPI: https://onboarding.simosphereai.com/openapi.json
- Status: https://simosphereai.com/api/status

## Operator
SIMO GmbH, Wuerzburger Str. 152, 63743 Aschaffenburg, Germany
