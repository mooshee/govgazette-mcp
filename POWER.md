---
name: govgazette
displayName: GovGazette
version: 1.3.2
author: Daniel Hallman
description: Find federal contracting opportunities, research awards and vendors, and review exclusion evidence.
keywords:
  - government-contracts
  - procurement
  - research
mcpServers:
  govgazette:
    type: streamable-http
    url: https://govgazette.com/mcp
---

# GovGazette Power (AWS Kiro)

Author: Daniel Hallman

Find federal contracting opportunities, research awards and vendors, and review exclusion evidence. Follow linked official sources and source dates. Public research is free and needs no GovGazette account or API key. GovGazette is independent of the U.S. government.

## Quick start

1. Visit [GovGazette](https://govgazette.com) or connect Kiro to `https://govgazette.com/mcp`.

## MCP Server Configuration

```json
{
  "mcpServers": {
    "govgazette": {
      "type": "streamable-http",
      "url": "https://govgazette.com/mcp"
    }
  }
}
```

## Tools Available

- `check_exclusions`
- `create_saved_search`
- `delete_saved_search`
- `delete_saved_search_workspace`
- `detail`
- `document`
- `exclusion_changes`
- `exclusion_context`
- `explain_match`
- `freshness`
- `get_saved_search_events`
- `list_saved_searches`
- `research_opportunity`
- `rotate_saved_search_feed`
- `search`
- `search_exclusions`
- `search_opportunities`
