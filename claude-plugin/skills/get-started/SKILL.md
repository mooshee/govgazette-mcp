---
name: get-started
description: Start using GovGazette after installation or when the user asks how to research federal opportunities, awards, vendors or exclusion evidence.
---

# Start federal contract research

Author: Daniel Hallman

## Quick start

Open [GovGazette](https://govgazette.com) in your browser or connect your assistant to `https://govgazette.com/mcp`. Public research is free and needs no account or key. Use the connected GovGazette MCP tools; if they are unavailable, explain the connection issue briefly instead of pretending to have searched.

If the user already supplied a research question, continue with it. Otherwise ask one concise question about their work, industry, location or agency of interest. Do not require an industry code before helping.

For an opportunity question, use `search_opportunities` with their keywords and supported filters, starting with three results. Read `freshness` when current dates matter. Carry the returned exact `id` and `generation` into `research_opportunity` for a selected result. Lead with useful findings, the response deadline and two dated links: the GovGazette record and official source. Active source status does not prove that a deadline is still open.

Use the contract-research or exclusion-review skill for the corresponding question. State unavailable information plainly. Do not infer eligibility, an incumbent or exclusion clearance.

Keep private saved searches optional. Do not provision a workspace merely because the plugin was installed. Only create or change a saved search when the user explicitly requests it and the host has a secure authenticated connection. Never request credentials in chat, and never submit bids or contact agencies.
