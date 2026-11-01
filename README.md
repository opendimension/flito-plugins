# Flito plugins

`flito/` is the Flito plugin for Claude (claude.ai, the desktop app, Cowork and Claude Code) and for ChatGPT and Codex. One folder serves both:

- Claude reads `.claude-plugin/plugin.json` and `.mcp.json`.
- ChatGPT and Codex read `plugin.json` and `mcp.json`.
- Both read the skills in `skills/`.

Its MCP connection is `https://flito.ai/mcp`: the shared sign-in in front of every Flito, which lives in the website repo (`lib/connect`). `services/api/test/flito-plugin.test.ts` keeps the skills in line with the MCP tools and the ask-first rules.

To hand the plugin to a store or an org catalog, zip it from inside the folder:

    cd plugins/flito && zip -r ../flito.zip . -x '.DS_Store'

`.claude-plugin/marketplace.json` makes this folder a Claude marketplace once it sits at the root of a public repo.
