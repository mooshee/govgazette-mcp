# GovGazette for Microsoft 365 Copilot

This declarative agent uses GovGazette's hosted MCP server for public, source-backed federal contract research. It pins the public read tools so the private saved-search action is not offered to Copilot.

The three JSON files and two PNG icons in this folder form the app package. The ready-to-upload archive is [govgazette-m365.zip](govgazette-m365.zip). Validate it with Microsoft 365 Agents Toolkit before sideloading or submitting it to Partner Center. The `developer.name` must match the verified publisher in Partner Center.

```sh
cd microsoft-365
zip -j govgazette-m365.zip manifest.json declarativeAgent.json ai-plugin.json color.png outline.png
atk validate --package-file govgazette-m365.zip
```

The plugin pins the 11 public read tools from the hosted MCP server. Refresh those definitions when the hosted tool contract changes.

Sources: [Microsoft's agent publishing guide](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/publish), [MCP plugin schema](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-manifest-2.4), [app package requirements](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agents-are-apps).
