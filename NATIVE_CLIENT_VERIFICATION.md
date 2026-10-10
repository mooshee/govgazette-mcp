# Verified GovGazette client behavior

Author: Daniel Hallman

Checked October 10, 2026 against the deployed GovGazette server. These are bounded operator QA checks. They do not establish customer use, demand, eligibility or complete source freshness.

## Catalog and protocol

The [live catalog](https://govgazette.com/api/v1/mcp/tools.json) exposes 17 separate operations with descriptions, input schemas, output schemas and safety annotations. Public research is available at `https://govgazette.com/mcp`; private saved searches use a separately authenticated connection.

| Public research | Private saved searches |
| --- | --- |
| `search_opportunities`, `research_opportunity`, `search`, `detail`, `document`, `freshness`, `explain_match`, `search_exclusions`, `check_exclusions`, `exclusion_context`, `exclusion_changes` | `create_saved_search`, `list_saved_searches`, `get_saved_search_events`, `rotate_saved_search_feed`, `delete_saved_search`, `delete_saved_search_workspace` |

The old `saved_searches` operation multiplexer is removed. Private operations remain unavailable without authenticated access. Discover the hosted catalog instead of copying an older directory scan or guessing an operation's inputs.

The server accepts the current `2026-07-28` discovery and request metadata contract and retains legacy protocol compatibility. Current responses include structured results with bounded text summaries; legacy responses retain complete JSON in text content. Neither representation makes a retained snapshot current government data.

## Observed native checks

| Client and route | Observed result | Limit |
| --- | --- | --- |
| Codex CLI 0.153.2, public research | Three actual MCP calls completed: `search_opportunities` → `detail` → `document`. The assistant received source URLs, source dates, generation and the selected notice's missing deadline. | Codex negotiated a legacy protocol. This is legacy native-client proof, not current-protocol proof. |
| mcporter 0.13.6 with MCP SDK 2.0.0, public research | Pinned `2026-07-28`; current discovery and tool listing succeeded, followed by `search_opportunities` → `detail` → `document`. The CLI exposed the structured results, including matching generation, source URLs and dates, deadline and a bounded document excerpt. | A controlled SDK client check. It does not establish that every host forwards structured results. |
| Codex, private OAuth QA | A fresh native authorization flow completed, then an actual `list_saved_searches` call returned an empty workspace. The QA grant was revoked and scoped local credentials cleaned up. | No saved search was created. A signed HTTP check confirmed rejection after revocation; a separate native negative attempt did not produce a typed native rejection and is not counted as proof. |
| ChatGPT, private OAuth QA | The native authorization flow completed; two successful `list_saved_searches` results returned an empty workspace. The QA grant and session were revoked and the temporary connection removed. | No saved search was created. The host made two calls despite a one-call prompt. Its protocol version was not established. |

Public QA checks also covered the retained document continuation path and missing, invalid and stale request context. A browser or CLI exit code alone was not counted as a successful tool result. Private evidence stays outside this public package; no tokens, account identifiers or user-entered private text are included here.

## Using the results

Start with a few results. Carry exact returned IDs and generation into related reads; preserve the supplied continuation offset for long retained notices. On a stale generation response, repeat the search before continuing. Follow official links for complete solicitation attachments and current requirements.

Report source dates and unavailable fields. An active notice can have an expired response deadline; a missing deadline is unknown. Similar awards do not establish an incumbent. Exclusion matches require identifier review, and a no-match result is not clearance.

Recipes for other hosts in the [README](README.md) describe setup, not observed task completion. The reviewed OpenAI package still needs an accepted upload, fresh hosted-tool scan, review submission and approval before it can become a public listing.
