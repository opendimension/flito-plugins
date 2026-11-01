---
name: email-reply
description: Read a conversation in the Flito inbox, draft a reply for the user to check, and send it only when told to. Use when the user asks to reply to, answer or follow up on an email.
---

# Email reply

1. Find the thread with `find_email_threads` by person, company or words, and read it with `read_email_thread`.
2. Draft a short, plain reply that says what the user wants, and show it in the chat.
3. Only if the user says to send it, use `send_email` with the threadId, to the people on the thread. Nothing goes out before their yes, and never to anyone else.
