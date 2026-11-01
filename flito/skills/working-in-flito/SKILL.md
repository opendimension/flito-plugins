---
name: working-in-flito
description: How to work in a Flito CRM through the Flito tools, and the rules for making changes there. Use whenever the user asks about their customers, companies, contacts, deals, leads, quotes, invoices, tasks, pipeline or CRM email in Flito.
---

# Working in Flito

Flito is the user's CRM. Its tools come from the Flito connection in this plugin, which signs the user in to their own Flito.

## Finding things

- Start with `search` for a name, email, phone, domain or number, then open the record with `fetch`.
- For lists with filters use `find_companies`, `find_contacts`, `find_deals`, `find_leads`, `find_quotes` and `find_invoices`.
- For "how many" or "how much" questions use `aggregate_records` or `pipeline_summary` rather than counting a list.
- For one company's whole picture use `get_account_summary`. For one deal use `check_deal`.
- For anything these tools don't cover, find a capability with `list_capabilities` and run it with `run_capability`.
- Link every record you mention. The tools' answers carry the links.

## Making changes

- You act as the user: changes you make run at once, under their name, and each one is kept in the record’s history with who made it, where the CRM can undo it.
- ASK FIRST. Before any of these, show the user exactly what will happen (who an email goes to, its subject and full text; the quote’s lines and total; which records and what changes) and wait for a clear yes in this chat: sending anything to people (emails, quotes for signature, sequences); creating a quote or changing its lines or prices; deleting, archiving or merging anything; changing more than 5 records at once; anything that spends credits; and settings, pipelines or automations.
- JUST DO IT. Other changes the user plainly asked for need no extra question: add a note or task, complete a task, update a field to the value they gave, move a deal to the stage they named, and add a company, contact, lead or deal (after checking it is not already on file). Then say what you did, with the link.
- If you are not sure the user asked for a change, ask. Never say something is done unless the tool’s answer shows it was.

## Answering

- Lead with what the user asked. Keep it short.
- Use the CRM's own names for stages, fields and records.
- If the Flito tools aren't connected, tell the user to connect Flito and sign in to their own Flito.
