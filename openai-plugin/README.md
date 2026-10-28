# GovGazette OpenAI review package

Author: Daniel Hallman

This directory retains the existing OpenAI app's package identity. The portable plugin in [`../plugin/`](../plugin/) remains `govgazette`; the OpenAI review package remains `app-6ab4095478448191842615fa4f3ce702`. Both are version 1.3.4 and connect public research to `https://govgazette.com/mcp` without authentication. Read the [release notes](https://github.com/mooshee/govgazette-mcp/releases/tag/v1.3.4) for this copy update.

The review package contains only `plugin.json`, `mcp.json` and the existing 512-pixel icon. It preserves the approved developer identity, existing category and capability selection, policy links, five positive review cases, three unsupported-action cases and the existing public demo. The demo shows a September 23 research task; it does not demonstrate the October 10 private OAuth flow or current protocol negotiation.

Build the ZIP from this directory so the existing app directory is the archive root:

```sh
ouch compress app-6ab4095478448191842615fa4f3ce702 /absolute/output/govgazette-openai-1.3.4.zip
ouch list /absolute/output/govgazette-openai-1.3.4.zip
uu-sha256sum /absolute/output/govgazette-openai-1.3.4.zip
```

Do not include this README, private account configuration, credentials, QA captures or operator logs in the upload. The hosted MCP catalog supplies the current tools and schemas; the ZIP does not freeze or replace that catalog.

On October 10, a retry in the existing OpenAI management entry was blocked before a successor draft was created: its MCP configuration was unavailable. This package still needs an accepted upload, a fresh tool scan, and provider review in that existing entry. It has not been submitted, approved, or publicly listed. Do not create a replacement app to work around that state.

See [distribution status](../DISTRIBUTION.md) and [verified client behavior](../NATIVE_CLIENT_VERIFICATION.md). A working developer-mode connection is separate from a public directory listing.
