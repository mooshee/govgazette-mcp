# GovGazette distribution

Author: Daniel Hallman

Package copy updated October 28, 2026. Provider review observations below were last checked October 10 unless stated otherwise. A package, submission, approval, public listing, and working research task are different milestones.

## Public routes

| Route | Evidence and scope |
| --- | --- |
| Portable plugin and host setup | [Public source package](plugin/) and [host recipes](README.md). Public research is free over Streamable HTTP; no account or key is required. |
| MCP Registry | The existing entry is `io.github.mooshee/govgazette`. Check the [registry API](https://registry.modelcontextprotocol.io/v0.1/servers/io.github.mooshee%2Fgovgazette/versions/latest) for its latest published version and status. |
| Glama | [GovGazette page](https://glama.ai/mcp/servers/mooshee/govgazette-mcp) is publicly visible. A directory page does not prove every native host has completed a research task. |
| Smithery | [Existing GovGazette page](https://smithery.ai/servers/daniel-hallman/govgazette). A prior scan may lag the live catalog; check its tool inventory before relying on it. |
| ClawHub | Existing [contract research](https://clawhub.ai/mooshee/skills/govgazette-contract-research) and [exclusion review](https://clawhub.ai/mooshee/skills/govgazette-exclusion-review) skills. Installing a skill alone does not connect MCP. |
| ChatGPT and Codex directory | Not publicly published at the October 10 check. The 1.3.4 package contains revised copy and preserves the existing app identity; it still requires provider review. Developer-mode research is a separate route. |
| Hermes catalog | [Existing catalog proposal](https://github.com/NousResearch/hermes-agent/pull/120612) remains under review. Direct portable installation is documented separately. |

## ChatGPT package and review

The [portable package](plugin/) includes `plugin.json`, one remote `mcp.json`, four skills, and full-resolution icons. The separate [OpenAI review package](openai-plugin/) preserves the existing app identity and downloaded release layout: `plugin.json`, `mcp.json`, and its icon. It includes no skills or private credentials. On October 28, the public connection listed 11 research tools with individual descriptions, schemas, and annotations. Public research needs no credentials. Private saved-search operations are separate and require authenticated access and explicit user intent.

OpenAI's [ZIP submission guide](https://developers.openai.com/plugins/deploy/submission) separates uploaded metadata/skills from hosted MCP scans, review submission and publication. The [package field reference](https://developers.openai.com/plugins/build/plugins) defines listing, review and onboarding fields. Hosted tool updates are automatically checked after initial publication; this does not make an unapproved package public.

## Acceptance

See [verified client behavior](NATIVE_CLIENT_VERIFICATION.md) for the October 10 native Codex, current-protocol SDK and private OAuth QA results and their limits. Other host setup recipes remain unverified task paths unless separately observed.

Connect in a fresh host context, discover tools, search a small result set, research a returned record with its exact ID and generation, and follow an official source link. Check actual deadlines rather than treating an active flag as an open response window. Cite source dates. A successful tool execution is not proof that another user's client received or used its result.

Do not infer an incumbent from similar awards or determine eligibility from exclusion evidence. [Privacy](https://govgazette.com/privacy), [terms](https://govgazette.com/terms) and [support](https://github.com/mooshee/govgazette-mcp/issues) remain available independently of directory review.
