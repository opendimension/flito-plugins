---
name: log-activity
description: Log a call, meeting or note on the right Flito records and add follow-up tasks. Use when the user says what happened with a customer, or asks you to note something or set a reminder.
---

# Log activity

1. Find the records it is about with `search`: the company, contact, deal or lead.
2. Use `add_note` with what happened, in the user's words, on the most specific record (a deal before its company).
3. If there is a next step, use `create_task` with a clear title, the due date and the record.
4. If the user named a new stage, use `update_deal_stage`. If they gave a new value for a field, use `update_record`.
5. Say what you logged, with links. These are plain changes: when the user asked for them, they need no extra question.
