# Dr. Canary plugins

Dr. Canary plugins for AI assistants, published by SCAI LLC.

## Plugins

| Plugin | What it does |
| --- | --- |
| [dr-canary](plugins/dr-canary/) | Bring Dr. Canary customer journey QA into your assistant: find UX bugs in connected websites and web apps, review browser evidence, prepare a developer fix brief, save focused checks and follow supported rechecks. |

## Install in Claude Code

1. Add this repository as a marketplace and install the plugin:

   ```
   /plugin marketplace add siteclarity/dr-canary-plugins
   /plugin install dr-canary@dr-canary-plugins
   ```

2. Connect your Dr. Canary account from the plugin's Connectors tab.
3. Follow the [plugin guide](plugins/dr-canary/README.md) for sign-in and permissions.

## What is in the plugin

- **Connector:** the hosted Dr. Canary MCP server at `https://www.drcanary.com/api/mcp/`, with OAuth sign-in.
- **Skills:**
  - `report-review` explains existing reports and evidence.
  - `site-test` saves focused checks and follows supported rechecks.
- **No scripts, hooks or local servers.**

## Repository layout

```
.claude-plugin/marketplace.json   Marketplace entry for this repository
plugins/dr-canary/
  .claude-plugin/plugin.json      Plugin manifest
  .mcp.json                       Hosted MCP server reference
  README.md                       Plugin guide and directory listing text
  assets/icon.png                 Plugin icon
  skills/report-review/           Skill and its reference notes
  skills/site-test/               Skill and its reference notes
```

## Support

- [Connection guide](https://www.drcanary.com/mcp/)
- [Connection troubleshooting](https://www.drcanary.com/mcp/troubleshooting/)
- [Privacy policy](https://www.drcanary.com/legal/privacy/)
- [Terms of service](https://www.drcanary.com/legal/terms/)

## License

- Published by SCAI LLC under the [Apache License 2.0](LICENSE).
- The license does not grant permission to use the Dr. Canary name or logo.
- Use of the Dr. Canary service is governed by its [Terms of service](https://www.drcanary.com/legal/terms/).
