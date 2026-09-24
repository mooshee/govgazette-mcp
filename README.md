# GovGazette: federal contract research with sources

[![GovGazette MCP server quality and maintenance on Glama](https://glama.ai/mcp/servers/mooshee/govgazette-mcp/badges/score.svg)](https://glama.ai/mcp/servers/mooshee/govgazette-mcp)

<!-- mcp-name: io.github.mooshee/govgazette -->

Find federal opportunities, research awards and vendors, and review exclusion evidence in your AI assistant. Public research is free and needs no GovGazette account or API key.

[Watch a short ChatGPT demo](media/chatgpt-demo.mp4) showing source-backed opportunity research.

## Set up your agent

Choose your agent below. For clients that ask for a server address, use **https://govgazette.com/mcp** with **Streamable HTTP** and **no authentication**.

When editing a configuration file, merge the GovGazette entry with your existing settings. Reload the client and enable its tools for your conversation.

<details>
<summary><strong>Claude Code</strong></summary>

Install the plugin:

```sh
claude plugin marketplace add mooshee/govgazette-mcp
claude plugin install govgazette@govgazette
```

It includes contract research and exclusion review skills. Start a new session after installation.

To connect just the MCP tools:

```sh
claude mcp add --transport http govgazette https://govgazette.com/mcp
```

[Provider setup guide](https://code.claude.com/docs/en/mcp)

</details>

<details>
<summary><strong>Codex</strong></summary>

Run:

```sh
codex mcp add govgazette --url https://govgazette.com/mcp
```

Or add this to `~/.codex/config.toml`:

```toml
[mcp_servers.govgazette]
url = "https://govgazette.com/mcp"
```

[Provider setup guide](https://developers.openai.com/learn/docs-mcp)

</details>

<details>
<summary><strong>ChatGPT</strong></summary>

For a custom MCP connection, use ChatGPT developer mode:

1. Enable developer mode in **Settings → Security and login**, if available in your workspace.
2. Open **ChatGPT Plugins**, select the **+** button, and create a plugin named **GovGazette** with MCP server URL `https://govgazette.com/mcp` and no authentication.
3. Enable GovGazette in a conversation and try the example below.

Developer-mode access depends on your plan and workspace settings.

[Provider setup guide](https://developers.openai.com/plugins/deploy/connect-chatgpt)

</details>

<details>
<summary><strong>Claude / Cowork / Desktop</strong></summary>

Open **Customize → Connectors**, select **+ → Add custom connector**, name it named **GovGazette**, and use:

```text
https://govgazette.com/mcp
```

Leave authentication unset for public research, then enable the connector in your conversation. Custom connector access depends on your plan and workspace settings.

[Provider setup guide](https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp)

</details>

<details>
<summary><strong>Gemini CLI</strong></summary>

Install the extension:

```sh
gemini extensions install https://github.com/mooshee/govgazette-mcp
```

It connects GovGazette and includes guidance for research with official sources. Restart Gemini CLI after installation.

Or merge this into your Gemini CLI `settings.json`:

```json
{
  "mcpServers": {
    "govgazette": {
      "httpUrl": "https://govgazette.com/mcp"
    }
  }
}
```

[Provider setup guide](https://geminicli.com/docs/tools/mcp-server/)

</details>

<details>
<summary><strong>Antigravity CLI / IDE</strong></summary>

Clone this repository and install the [Antigravity plugin](antigravity-plugin/):

```sh
git clone https://github.com/mooshee/govgazette-mcp.git
cd govgazette-mcp
agy plugin install ./antigravity-plugin
agy plugin list
```

The plugin connects GovGazette and includes contract research and exclusion review skills. For Antigravity 2.0 or the standalone IDE, place `antigravity-plugin/` at `.agents/plugins/govgazette/` in a workspace or `~/.gemini/config/plugins/govgazette/` globally. Public research needs no account or key.

[Provider setup guide](https://www.antigravity.google/docs/plugins/)

</details>

<details>
<summary><strong>Hermes Agent</strong></summary>

Install the portable plugin from this repository's `plugin/` directory:

```sh
hermes plugins install mooshee/govgazette-mcp/plugin --no-enable
hermes plugins enable govgazette
hermes mcp test govgazette
```

Or connect just the MCP tools by merging this into `~/.hermes/config.yaml`:

```yaml
mcp_servers:
  govgazette:
    url: "https://govgazette.com/mcp"
```

Use one method to avoid registering the same server twice. Public research needs no GovGazette key.

[Provider setup guide](https://hermes-agent.nousresearch.com/docs/developer-guide/plugins/)

</details>

<details>
<summary><strong>Cursor</strong></summary>

Merge this into `.cursor/mcp.json`, then enable the server:

```json
{
  "mcpServers": {
    "govgazette": {
      "url": "https://govgazette.com/mcp"
    }
  }
}
```

[Provider setup guide](https://prod.cursor.com/help/customization/mcp)

</details>

<details>
<summary><strong>GitHub Copilot / VS Code</strong></summary>

Merge this into `.vscode/mcp.json`, start the server, and enable its tools in agent mode:

```json
{
  "servers": {
    "govgazette": {
      "type": "http",
      "url": "https://govgazette.com/mcp"
    }
  }
}
```

[Provider setup guide](https://code.visualstudio.com/docs/agent-customization/mcp-servers)

</details>

<details>
<summary><strong>Gemini Spark (web and mobile)</strong></summary>

With a personal Google account in the US, open Gemini Spark → Connected Apps → Custom apps and add `https://govgazette.com/mcp`. Then mention `@GovGazette` in a prompt. Google currently supports custom app setup on the web; the connection also works in its mobile app.

[Google setup guide](https://support.google.com/gemini/answer/17209137)

</details>

<details>
<summary><strong>Microsoft 365 Copilot</strong></summary>

The [declarative agent package](microsoft-365/) connects to GovGazette's public research tools. A Microsoft 365 tenant with custom app upload and Copilot access can validate and sideload it.

[Microsoft publishing guide](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/publish)

</details>

<details>
<summary><strong>Devin CLI / Desktop / cloud</strong></summary>

Install the [portable GovGazette plugin](plugin/) from this repository:

```sh
devin plugins install mooshee/govgazette-mcp#plugin
```

The plugin includes the public MCP connection and contract research and exclusion review skills. After installation, connect GovGazette in **Customize → MCPs** if Devin asks, then check its tools in a new session. A Devin account is required to manage CLI plugins.

[Plugin setup guide](https://docs.devin.ai/cli/extensibility/plugins/overview) · [MCP connection guide](https://docs.devin.ai/work-with-devin/mcp)

</details>

<details>
<summary><strong>Windsurf / Cascade</strong></summary>

Open the MCP configuration from Cascade and merge this server:

```json
{
  "mcpServers": {
    "govgazette": {
      "serverUrl": "https://govgazette.com/mcp"
    }
  }
}
```

[Provider setup guide](https://docs.devin.ai/desktop/cascade/mcp)

</details>

<details>
<summary><strong>Cline</strong></summary>

Open Cline’s MCP server settings and add this Streamable HTTP connection:

```json
{
  "mcpServers": {
    "govgazette": {
      "type": "streamableHttp",
      "url": "https://govgazette.com/mcp",
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

[Provider setup guide](https://docs.cline.bot/mcp/mcp-overview)

</details>

<details>
<summary><strong>Continue</strong></summary>

Add this entry to the `mcpServers` list in your Continue configuration:

```yaml
mcpServers:
  - name: GovGazette
    type: streamable-http
    url: https://govgazette.com/mcp
```

[Provider setup guide](https://docs.continue.dev/customize/deep-dives/mcp)

</details>

<details>
<summary><strong>OpenCode</strong></summary>

Merge this into `opencode.json`:

```json
{
  "mcp": {
    "govgazette": {
      "type": "remote",
      "url": "https://govgazette.com/mcp",
      "enabled": true
    }
  }
}
```

[Provider setup guide](https://opencode.ai/docs/mcp-servers/)

</details>

<details>
<summary><strong>Kiro</strong></summary>

Merge this into the MCP configuration for your Kiro IDE or CLI:

```json
{
  "mcpServers": {
    "govgazette": {
      "url": "https://govgazette.com/mcp"
    }
  }
}
```

[Provider setup guide](https://kiro.dev/docs/mcp/configuration/)

</details>

<details>
<summary><strong>OpenClaw</strong></summary>

Use an OpenClaw version with the MCP registry feature. Add this to its configuration and follow the provider guide to run a connection probe:

```json
{
  "mcp": {
    "servers": {
      "govgazette": {
        "url": "https://govgazette.com/mcp",
        "transport": "streamable-http"
      }
    }
  }
}
```

[Provider setup guide](https://docs.openclaw.ai/cli/mcp/registry)

</details>

<details>
<summary><strong>Perplexity</strong></summary>

Add a custom remote connector named **GovGazette** with this URL and open authentication:

```text
https://govgazette.com/mcp
```

Enable it for your research. Custom connector access depends on your plan and workspace settings.

[Provider setup guide](https://www.perplexity.ai/en-GB/changelog/what-we-shipped---march-13-2026)

</details>

<details>
<summary><strong>Grok API</strong></summary>

Add this remote MCP tool to your Grok API request. Use the API integration for this setup:

```json
{
  "type": "mcp",
  "server_url": "https://govgazette.com/mcp",
  "server_label": "govgazette",
  "allowed_tools": [
    "search_opportunities",
    "research_opportunity",
    "search",
    "detail",
    "freshness",
    "check_exclusions"
  ]
}
```

[Provider setup guide](https://docs.x.ai/developers/tools/remote-mcp)

</details>

<details>
<summary><strong>LM Studio</strong></summary>

Open **Program → Install → Edit mcp.json** and merge this server. Choose a model that supports tools:

```json
{
  "mcpServers": {
    "govgazette": {
      "url": "https://govgazette.com/mcp"
    }
  }
}
```

[Provider setup guide](https://beta.lmstudio.ai/docs/app/mcp)

</details>

<details>
<summary><strong>Open WebUI / Ollama</strong></summary>

In the administrator settings, add an external tool server:

```text
Name: GovGazette
Type: MCP (Streamable HTTP)
URL: https://govgazette.com/mcp
Authentication: None
```

Enable it for your chat and select a model that supports tools. For Ollama models, configure the connection in Open WebUI.

[Provider setup guide](https://docs.openwebui.com/features/extensibility/mcp/)

</details>

<details>
<summary><strong>Amazon Q Developer</strong></summary>

In the IDE tools panel, add a server named **GovGazette**, choose **HTTP**, enter `https://govgazette.com/mcp`, and save. Review and enable the tools you want to use.

[Provider setup guide](https://docs.aws.amazon.com/amazonq/latest/qdeveloper-ug/mcp-ide.html)

</details>

## Try it

> Find three active software notices in industry 541512. Research one, cite its official source and date, and check whether the response deadline is still open.

You can also ask your agent to research a vendor by its Unique Entity Identifier (UEI), explain an industry code, or review a possible exclusion match.

## Save a search

[Create a private workspace](https://govgazette.com/monitor) to follow changes in an inbox or feed. To manage saved searches through an agent, store your workspace key in the client’s secret-header settings as `Authorization: Bearer YOUR_WORKSPACE_KEY`. Keep it out of prompts and shared configuration files.

## Research with care

Check the official source and its date. An active notice can have a deadline that has passed. Similar awards do not establish an incumbent, and an exclusion search does not determine eligibility. Consult official attachments for complete solicitation requirements. GovGazette is independent of the U.S. government.

[Website](https://govgazette.com) · [API reference](https://govgazette.com/api/v1/openapi.json) · [Agent guide](https://govgazette.com/llms.txt) · [Privacy](https://govgazette.com/privacy) · [Support](https://github.com/mooshee/govgazette-mcp/issues) · [MCP Registry](https://registry.modelcontextprotocol.io/?q=io.github.mooshee%2Fgovgazette)
