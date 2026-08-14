# GovGazette MCP Server

<!-- mcp-name: io.github.mooshee/govgazette -->

GovGazette is a hosted MCP server for U.S. federal contract research and pursuit monitoring.

Connect with Streamable HTTP:

```text
https://govgazette.com/mcp
```

The five research tools work without an account:

- `search_opportunities`
- `get_opportunity`
- `get_opportunity_comps`
- `get_vendor`
- `get_vendor_awards`

OAuth 2.1 with PKCE unlocks account-scoped monitoring:

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
