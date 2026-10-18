---
name: sweeping-a-board
description: How to go through every open item quickly and correctly
metadata:
  type: reference
---

- A whole project read can be too big for one answer and spill to a file. Parse that file (TOML) instead of reading it by eye. Count the open items by state and by epic first.
- Split a big sweep by epic among helpers, roughly 30 items each, and give every helper the same rules: how to find evidence, what each state means, no whole-project edits, and to write a table and report back.
- Check their calls before reporting, above all closures made on judgement (a fix with no proven cause, a question nobody answered).
- Then do the epics yourself:
  - re-date the ones whose targets have passed;
  - an epic whose tasks are all done is done;
  - a task left under a finished epic, or under none, moves to a live epic.
- To wait on helpers, watch for the files they write rather than the inbox, which wakes on unrelated posts.
- Finish with one page for the person: what was closed (with evidence), what's left by epic, and the decisions that are theirs.

**Why:** boards drift. Work ships without its item closing, and dates pass unnoticed.
**How to apply:** sweep whenever asked, and on the scheduled morning wake. Related: [[closing-with-evidence]], [[tool-quirks]].
