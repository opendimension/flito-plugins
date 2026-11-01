# Flito plugins

The Flito plugin puts your Flito CRM in Claude and ChatGPT: the Flito connection, and skills for the work people do most, in one install.

## What's in it

- **The Flito connection** at `https://flito.ai/mcp`. It works for every Flito. The first time you use it, you enter your Flito's address (such as crm.yourcompany.com), sign in there and choose what the app can do.
- **Eight skills:** working in Flito, account summary, pipeline review, deal check, quote, log activity, my day and email reply. In Claude Code and Cowork they also run as commands, such as `/flito:pipeline-review`.

## Install

**Claude Code**

```bash
claude plugin install flito --marketplace opendimension/flito-plugins
```

Inside Claude Code, the same works as `/plugin install flito --marketplace opendimension/flito-plugins`.

**Claude (web and desktop):** Customize, Plugins, Add, Add marketplace, then enter `opendimension/flito-plugins` and add Flito. Open the plugin's Connectors tab and connect Flito.

**Codex**

```bash
codex plugin marketplace add opendimension/flito-plugins
```

**ChatGPT:** until Flito is in the ChatGPT plugin directory, add the connection on its own. In Settings, Apps, Advanced settings, turn on Developer mode, then Create: name it Flito, use the server address `https://flito.ai/mcp` and choose OAuth.

## How changes work

The app works as you, with no more access than you have. Before anything risky, such as sending an email or a quote, creating a quote, deleting, or changing many records at once, it shows you what will happen and waits for your yes. Plain changes you ask for, such as a note or a task, it just makes. Every change is kept in the record's history, where Flito can undo it.

## More

- Developer docs: https://flito.ai/docs
- The MCP connection: https://flito.ai/docs/mcp

MIT licensed.
