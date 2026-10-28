---
name: get-started
description: Help a user start researching federal opportunities, awards, vendors, or exclusion records with GovGazette.
---

# Start federal contract research

Author: Daniel Hallman

## Connect

1. Open [GovGazette](https://govgazette.com) in your browser, or connect your assistant to `https://govgazette.com/mcp`. Public research is free and requires no account or API key.
2. Check that the GovGazette tools are available. If they are missing, explain the connection issue briefly; do not claim to have searched.

## Start a search

1. Use the user's research question if they already supplied one. Otherwise ask one short question about their work, industry, location, or agency of interest. An industry code is optional.
2. For opportunities, call `search_opportunities` with their keywords and supported filters. Start with three results.
3. Call `freshness` when current dates matter. An active source status does not prove that a response deadline is still open.
4. For a selected result, pass its exact `id` and returned `generation` to `research_opportunity`.
5. Lead with the useful findings and response deadline when available. Include dated links to the GovGazette record and official source. State missing information plainly.

Use `contract-research` or `exclusion-review` for the corresponding question. Do not infer eligibility, an incumbent, or exclusion clearance.

Private saved searches are optional. Do not create a workspace just because the plugin was installed. Create or change a saved search only when the user explicitly requests it and the host has a secure authenticated connection. Never request credentials in chat, submit bids, or contact agencies.

Built and maintained by [Moosh Works](https://mooshworks.com).
