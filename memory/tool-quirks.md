---
name: tool-quirks
description: Behaviours of the project tools that catch you out
metadata:
  type: reference
---

- An update must change a field or the state. A reason on its own is refused, so put the reason on the change it explains.
- A whole-project edit rewrites everything. Don't use it while other agents are editing items; use item-by-item updates.
- Searching for items shows only open ones unless you ask for closed ones too. Check both before filing, so you don't duplicate.
- A closed item's reason can't be edited later.
- "blocked" on an item only means something it needs is still open. Drop a need that no longer applies rather than leaving the item looking stuck.

**Why:** each of these has cost a re-do.
**How to apply:** read this before a big batch of edits. Related: [[sweeping-a-board]].
