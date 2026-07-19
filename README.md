# gitdealflow MCP server

VC deal-flow intelligence for AI agents. Search tracked startups by sector, city, or keyword; pull engineering momentum signals (commit velocity, contributor growth, new-repo spawning, deploy-frequency spikes) derived from public GitHub activity.

**Live endpoint:** `https://gitdealflow.com/api/mcp` (HTTP, MCP 2024-11-05)

Backed by the Startup Engineering Acceleration Dataset (DOI [10.5281/zenodo.19650920](https://doi.org/10.5281/zenodo.19650920)) and a deterministic 4-class signal classifier ([classifier repo](https://github.com/kindrat86/gitdealflow-signal-classifier)).

## Tools

| Tool | What it does |
|---|---|
| `search_startups` | Search tracked startups by sector, city, or keyword |
| `get_startup_signal` | Get engineering momentum signal for a specific startup |
| `list_sectors` | List all tracked sectors |
| `list_cities` | List all tracked cities |

## Usage

```json
{
  "mcpServers": {
    "gitdealflow": { "url": "https://gitdealflow.com/api/mcp" }
  }
}
```

MIT License. Free.
