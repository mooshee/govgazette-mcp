# GovGazette: federal contract research with sources

<!-- mcp-name: io.github.mooshee/govgazette -->

Find federal notices, build a cited research brief, research awards and vendors, and review exclusion evidence in your AI assistant. Public research is free and requires no GovGazette account or API key.

## Connect with MCP

Use Streamable HTTP at **https://govgazette.com/mcp**.

[Choose your client](https://govgazette.com/agents) for Codex, ChatGPT, Claude, Cursor, VS Code, Gemini CLI and other supported configuration formats. Each page separates setup instructions from actual native acceptance.

## Install the Claude Code plugin

```sh
claude plugin marketplace add mooshee/govgazette-mcp
claude plugin install govgazette@govgazette
```

Version 1.3.0 passed native Claude Code installation and connected to the live MCP server on September 23, 2026. End-to-end model research remains separately tracked. The plugin connects the hosted MCP server and includes `contract-research` and `exclusion-review` skills. This is GovGazette's own repository marketplace, not an Anthropic endorsement or curated marketplace listing.

## ChatGPT and Codex plugin

- [Download the portable plugin](https://govgazette.com/integrations/govgazette-plugin.zip): MCP connection, research skills and brand icon. Source: `plugin/`.
- [ChatGPT connector setup](https://govgazette.com/agents/chatgpt).
- [Codex setup](https://govgazette.com/agents/codex).

Custom GPT launch work is retired in favor of the plugin. Public OpenAI directory acceptance remains separate from the downloadable package.

## Try it

> Find three active software notices in industry 541512. Research one, cite the official source and its date, and check whether the response deadline is still open.

Public tools: `search`, `detail`, `freshness`, `document`, `explain_match`, `search_opportunities`, `research_opportunity`, `search_exclusions`, `check_exclusions`, `exclusion_context`, `exclusion_changes`.

`saved_searches` is separate and requires a private workspace bearer key. Create a workspace on the website; configure the key in your client's secret headers, never in prompts. The current service does not use the retired OAuth account-monitoring flow or send email alerts. Older releases described a different tool contract.

## Sources and limits

Follow the official source and source date. Active source status does not mean the deadline is open. Similar awards do not establish an incumbent. Name-only exclusion matches are possible matches, and no match is not clearance. Original attachments are not automatically extracted. GovGazette is independent of the U.S. government.

- [Public API / OpenAPI](https://govgazette.com/api/v1/openapi.json)
- [Agent contract](https://govgazette.com/llms.txt)
- [Privacy](https://govgazette.com/privacy)
- [Official MCP Registry](https://registry.modelcontextprotocol.io/?q=io.github.mooshee%2Fgovgazette)

This repository distributes metadata and integration packages. The hosted application source is maintained separately. Version 1.3.0 updates discovery metadata and plugin packaging for the current service.
