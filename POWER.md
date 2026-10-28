---
name: govgazette
displayName: GovGazette
version: 1.3.4
author: Daniel Hallman
description: Find federal contract opportunities, research awards and vendors, and review exclusion records.
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

Author: Daniel Hallman ([Moosh Works](https://mooshworks.com))

Find federal contract opportunities, research awards and vendors, and review exclusion records. Check linked official sources and their dates. Public research is free and requires no account or API key. GovGazette is independent of the U.S. government.

## Quick start

1. Open [GovGazette](https://govgazette.com) to browse records, or connect Kiro to `https://govgazette.com/mcp`.
2. Confirm that Kiro lists the research tools, then ask for a small set of opportunities.
3. Check the returned source dates and official links before relying on a record.

Private saved-search actions require an authenticated workspace and the user's request. Keep credentials out of chat and shared files.

Built and maintained by [Moosh Works](https://mooshworks.com).

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

## Public research tools

- `check_exclusions`
- `detail`
- `document`
- `exclusion_changes`
- `exclusion_context`
- `explain_match`
- `freshness`
- `research_opportunity`
- `search`
- `search_exclusions`
- `search_opportunities`

## Private saved-search tools

These tools require a separate authenticated workspace. Discover the tools
available to that connection before using them.

- `create_saved_search`
- `list_saved_searches`
- `get_saved_search_events`
- `rotate_saved_search_feed`
- `delete_saved_search`
- `delete_saved_search_workspace`
