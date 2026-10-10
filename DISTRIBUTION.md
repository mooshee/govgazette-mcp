# GovGazette distribution

Author: Daniel Hallman

Status checked October 10, 2026. A package, submission, approval, public listing and working research task are different milestones.

## Public routes

| Route | Evidence and scope |
| --- | --- |
| Portable plugin and host setup | [Public source package](plugin/) and [host recipes](README.md). Public research is free over Streamable HTTP; no account or key is required. |
| MCP Registry | [Registry entry](https://registry.modelcontextprotocol.io/?q=io.github.mooshee%2Fgovgazette). Package releases use the existing publisher workflow; verify the registry version separately from Git tags. |
| Glama | [GovGazette page](https://glama.ai/mcp/servers/mooshee/govgazette-mcp) is publicly visible. A directory page does not prove every native host has completed a research task. |
| Smithery | [Existing GovGazette page](https://smithery.ai/servers/daniel-hallman/govgazette). A prior scan may lag the live catalog; check its tool inventory before relying on it. |
| ClawHub | Existing [contract research](https://clawhub.ai/mooshee/skills/govgazette-contract-research) and [exclusion review](https://clawhub.ai/mooshee/skills/govgazette-exclusion-review) skills. Installing a skill alone does not connect MCP. |
| ChatGPT and Codex directory | Not publicly published at this check. The corrected 1.3.1 package is prepared for review, not an approved directory listing. Developer-mode research is a separate route. |
| Hermes catalog | [Existing catalog proposal](https://github.com/NousResearch/hermes-agent/pull/120612) remains under review. Direct portable installation is documented separately. |

## ChatGPT package and review

The package includes `plugin.json`, one remote `mcp.json`, three skills and full-resolution icons. Every model-callable MCP operation is exposed individually with its description, input schema and annotations. Public research needs no credentials. Private saved-search operations are separate and require authenticated workspace access and explicit user intent.

OpenAI's [ZIP submission guide](https://developers.openai.com/plugins/deploy/submission) separates uploaded metadata/skills from hosted MCP scans, review submission and publication. The [package field reference](https://developers.openai.com/plugins/build/plugins) defines listing, review and onboarding fields. Hosted tool updates are automatically checked after initial publication; this does not make an unapproved package public.

## Acceptance

Connect in a fresh host context, discover tools, search a small result set, research a returned record with its exact ID and generation, and follow an official source link. Check actual deadlines rather than treating an active flag as an open response window. Cite source dates. A successful tool execution is not proof that another user's client received or used its result.

Do not infer an incumbent from similar awards or determine eligibility from exclusion evidence. [Privacy](https://govgazette.com/privacy), [terms](https://govgazette.com/terms) and [support](https://github.com/mooshee/govgazette-mcp/issues) remain available independently of directory review.
