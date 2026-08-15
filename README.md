# GovGazette MCP Server

<!-- mcp-name: io.github.mooshee/govgazette -->

GovGazette is a hosted MCP server for U.S. federal contract research and pursuit monitoring. Version 1.2.0 exposes 22 tools.

Connect with Streamable HTTP:

```text
https://govgazette.com/mcp
```

Seventeen research tools work without an account:

- `search_opportunities`
- `resolve_identifier`
- `lookup_reference`
- `get_opportunity`
- `get_opportunity_comps`
- `search_awards`
- `get_award`
- `search_vendors`
- `get_vendor`
- `get_vendor_awards`
- `get_opportunity_changes`
- `search_exclusions`
- `get_opportunity_extracted`
- `search_extracted_facts`
- `get_opportunity_documents`
- `find_recompetes`
- `get_market_summary`

OAuth 2.1 with PKCE unlocks five account-scoped monitoring tools:

- `get_watch_status`
- `save_opportunity_search`
- `update_saved_search`
- `track_opportunity`
- `update_tracked_opportunity`

The monitoring tools can create, update, and disable saved searches and tracked opportunities. They cannot delete records, change billing, or access another account.

## Links

- [Agent documentation](https://govgazette.com/agents?utm_source=github_mcp_repo&utm_medium=repository&utm_campaign=govgazette_agent_launch_2026_08)
- [OpenAPI document](https://govgazette.com/api/agent/openapi.json)
- [MCP protected resource metadata](https://govgazette.com/.well-known/oauth-protected-resource/mcp)
- [Official MCP Registry listing](https://registry.modelcontextprotocol.io/?q=io.github.mooshee%2Fgovgazette)

This repository contains public discovery metadata for the hosted service. It does not contain the GovGazette application source.
