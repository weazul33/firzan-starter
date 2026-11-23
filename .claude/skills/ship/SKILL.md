---
name: ship
description: Put a saved change on the live page.
disable-model-invocation: true
---

Read "Where it lives" in CLAUDE.md first.

At level 1 (my computer): say "Your page runs on your computer. /level-up puts it online, and we'll do that together in session 2." Stop.

At level 2 (GitHub):
1. Privacy check of every file that changed, not just docs/: the brief, NOTES.md, HABITS.md and reviews/ go live too. Merging puts all of them in the public project. Fix anything private first.
2. Make sure the latest change is saved (/save). If not, suggest it. A wrap-up commit from /wrapup already counts as saved.
3. Steps to go live, one at a time:
   - Press "Create PR" on the Changes card (or ask me to open a pull request). A pull request is a request to put this change on the live page.
   - Open it on GitHub. Click "Files changed" and read what's different. This is habit 4, read before you approve, on the real thing.
   - Before they merge, ask: "In a few words, what changed?" If they can say it, count habit 4 under "On my own". If they didn't look, count it under "Reminded" and ask them to look first. You can't see GitHub, so don't guess. Note what they told you in your moves log for the review. For any merge after the wrap-up commit from /wrapup, don't change HABITS.md: the scorecard is already committed, so a count then would be lost. If that merge has page changes, still ask the question as practice; if it's notes only, skip it.
   - Click "Merge pull request", then "Confirm merge".
4. The live page updates within about ten minutes. Ask them to open the link and confirm. If this merge only had notes and the review, say the page won't look different, and skip the check. After the wrap-up commit, don't count anything, habit 5 included.
5. If they don't want it live yet, that's fine: say the change stays on this session's branch and won't be there in the next session unless it's merged.
