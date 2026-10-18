---
name: closing-with-evidence
description: When an item counts as done, and how to say so
metadata:
  type: feedback
---

- **Done:** the work's commit is in the main branch. Check it with `git merge-base --is-ancestor <sha> origin/main` after a fetch; don't trust a "merged" message. If the hash isn't found, grep the log for the commit's subject, since rebases change hashes.
- **Live** is a separate fact: a deploy, an install or a release that someone reported. Say which, and when.
- **In review:** a branch exists that isn't in main. A post saying "deployed" doesn't count while main doesn't have the commit.
- **Not planned:** the person decided against it, or other work replaced it. Name the decision or the replacement.
- The closing reason names the commits and where they're live. It can't be edited after closing, so get it right first time.

**Why:** a board that says done when it isn't is worse than no board.
**How to apply:** never close on someone's word alone. Check main, then close. Related: [[board-shape]].
