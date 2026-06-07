<div align="center">

# SIMOSphere AI MCP Examples

**Model Context Protocol integration examples -- connect enterprise data sources with AI agents.**

[![smithery badge](https://smithery.ai/badge/simosphereai/simosphere-ai)](https://smithery.ai/servers/simosphereai/simosphere-ai)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

[English](#english) | [Deutsch](#deutsch)

</div>

---

## English

### Overview

Integration examples for the [SIMOSphere AI](https://simosphereai.com) MCP server. Connect enterprise data sources (CRM, ERP, SharePoint, DMS) with AI agents -- GDPR-compliant, EU-hosted.

Built by [SIMO GmbH](https://simo-online.com).

### MCP Server

| Property      | Value                                                                  |
| ------------- | ---------------------------------------------------------------------- |
| **URL**       | https://mcp.simosphereai.com                                           |
| **Transport** | Streamable HTTP                                                        |
| **Auth**      | Bearer token (API key)                                                 |
| **Server Card** | https://simosphereai.com/.well-known/mcp/server-card.json            |
| **Manifest**  | https://simosphereai.com/.well-known/mcp/manifest.json                 |

### Available Tools

| Tool                 | Description                                      |
| -------------------- | ------------------------------------------------ |
| `search_documents`   | Search SharePoint, DMS, local files              |
| `query_database`     | Read-only queries against Dynamics 365, ERP, CRM |
| `create_record`      | Create records in CRM/ERP systems                |
| `send_notification`  | Send via email, Teams, or Slack                  |

### Claude Desktop Configuration

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

### Cursor / VS Code Configuration

Add to your MCP settings:

- **Server URL:** `https://mcp.simosphereai.com`
- **Auth:** Bearer `sk-simo-your-key-here`

### Azure Marketplace

SIMOSphere M365 Governance is available on the [Microsoft Azure Marketplace](https://marketplace.microsoft.com/en-us/product/azure-application/simosimplemarketing1619635742390.simosphere-m365-governance-preview).

### Resources

- **Documentation:** [simosphereai.com/de/developers](https://simosphereai.com/de/developers)
- **MCP Spec:** [simosphereai.com/de/mcp-server](https://simosphereai.com/de/mcp-server)
- **OpenAPI Spec:** [api.simosphereai.com/openapi.json](https://api.simosphereai.com/openapi.json)
- **SDK:** [@simosphere/sdk on npm](https://www.npmjs.com/package/@simosphere/sdk)

---

## Deutsch

### Ueberblick

Integrationsbeispiele fuer den [SIMOSphere AI](https://simosphereai.com) MCP-Server. Verbinden Sie Unternehmensdatenquellen (CRM, ERP, SharePoint, DMS) mit KI-Agenten -- DSGVO-konform, gehostet in der EU.

Entwickelt von [SIMO GmbH](https://simo-online.com).

### MCP-Server

| Eigenschaft     | Wert                                                                   |
| --------------- | ---------------------------------------------------------------------- |
| **URL**         | https://mcp.simosphereai.com                                           |
| **Transport**   | Streamable HTTP                                                        |
| **Auth**        | Bearer-Token (API-Schluessel)                                          |
| **Server Card** | https://simosphereai.com/.well-known/mcp/server-card.json              |
| **Manifest**    | https://simosphereai.com/.well-known/mcp/manifest.json                 |

### Verfuegbare Tools

| Tool                 | Beschreibung                                         |
| -------------------- | ---------------------------------------------------- |
| `search_documents`   | Suche in SharePoint, DMS, lokalen Dateien            |
| `query_database`     | Lesende Abfragen gegen Dynamics 365, ERP, CRM        |
| `create_record`      | Datensaetze in CRM-/ERP-Systemen anlegen             |
| `send_notification`  | Benachrichtigungen per E-Mail, Teams oder Slack      |

### Claude-Desktop-Konfiguration

```json
{
  "mcpServers": {
    "simosphere": {
      "command": "npx",
      "args": ["-y", "@simosphere/mcp-client"],
      "env": {
        "SIMOSPHERE_API_KEY": "sk-simo-ihr-schluessel"
      }
    }
  }
}
```

### Cursor / VS Code Konfiguration

In Ihren MCP-Einstellungen hinterlegen:

- **Server-URL:** `https://mcp.simosphereai.com`
- **Auth:** Bearer `sk-simo-ihr-schluessel`

### Azure Marketplace

SIMOSphere M365 Governance ist im [Microsoft Azure Marketplace](https://marketplace.microsoft.com/en-us/product/azure-application/simosimplemarketing1619635742390.simosphere-m365-governance-preview) verfuegbar.

### Ressourcen

- **Dokumentation:** [simosphereai.com/de/developers](https://simosphereai.com/de/developers)
- **MCP-Spezifikation:** [simosphereai.com/de/mcp-server](https://simosphereai.com/de/mcp-server)
- **OpenAPI-Spezifikation:** [api.simosphereai.com/openapi.json](https://api.simosphereai.com/openapi.json)
- **SDK:** [@simosphere/sdk auf npm](https://www.npmjs.com/package/@simosphere/sdk)

---

## License / Lizenz

MIT -- Engineered at SIMO GmbH · Aschaffenburg, Germany
