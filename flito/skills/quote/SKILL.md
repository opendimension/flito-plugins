---
name: quote
description: Prepare a quote in Flito from what a customer asked for, show it, create it once the user agrees, and send it for signature when told to. Use when the user wants to quote, price, change or send a quote, including from a customer's email.
---

# Quote

1. Work out what the customer wants. If it came by email, find the thread with `find_email_threads` and read it with `read_email_thread`.
2. Use `draft_quote` to price it for the buyer. A draft saves nothing.
3. Show the user the lines, the totals, who it is for, where it bills and ships, and anything missing or flagged. If something is unclear, ask rather than guess.
4. Only after the user agrees, use `create_quote` with the same arguments. To add to a quote that already exists, use `add_quote_line`.
5. Only when the user says to send it, use `send_quote_for_signature`, after saying who it goes to.
6. Never say a quote was made or sent unless the tool's answer shows it.
