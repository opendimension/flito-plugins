# Flito

Work in your Flito CRM from Claude and ChatGPT. Ask about customers, deals, quotes, invoices, tasks and email in plain words, and the app does the CRM work for you, signed in to your own Flito.

## What's inside

- **The Flito connection** at `https://flito.ai/mcp`, which works for every Flito. The first time you use it, you enter your Flito's address (such as crm.yourcompany.com), sign in there and choose what the app can do.
- **Skills** for working in Flito, account summaries, pipeline reviews, deal checks, quotes, logging activity, planning your day and replying to email. In Claude Code and Cowork they also run as commands, such as `/flito:pipeline-review`.

## How changes work

The app works as you, with no more access than you have. Before anything risky, such as sending an email or a quote, creating a quote, deleting, or changing many records at once, it shows you what will happen and waits for your yes. Plain changes you ask for, such as a note or a task, it just makes. Every change is kept in the record's history, where Flito can undo it.

## Install

In Claude Code:

    /plugin install flito --marketplace opendimension/flito-plugins

Steps for Claude on the web and desktop, Codex and ChatGPT: https://github.com/opendimension/flito-plugins#install
