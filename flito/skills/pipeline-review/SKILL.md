---
name: pipeline-review
description: Review the Flito pipeline, with where the deals sit, what closes soon and what looks stuck. Use when the user asks about their pipeline, forecast, deals closing or deals at risk.
---

# Pipeline review

1. Use `pipeline_summary` for the totals by stage: count, amount and weighted amount.
2. Use `find_deals` with openOnly for the open deals closing in the next 30 days, or the period the user gives, largest first.
3. Use `find_deals` again for open deals that haven't been updated for a while.
4. Summarise: the total open and weighted value, what should close soon, and which deals look stuck and why. Include links.

To move a deal or add a task, follow the rules in the working-in-flito skill.
