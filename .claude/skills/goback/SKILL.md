---
name: goback
description: Put the page back to a saved version without deleting anything.
disable-model-invocation: true
---

Only the website (the docs folder) goes back. The brief, NOTES.md, HABITS.md and reviews/ stay as they are, so the scorecard and log keep counting.

1. Read "Where it lives" in CLAUDE.md. List the saved versions, newest first, in plain words: at level 1 the folders in versions/ with their NOTES line; at level 2 the recent saves (commits) on GitHub with their labels.
2. Ask which one to go back to. Suggest the newest.
3. Before changing anything, tell them in plain words what will come back and what they'll lose from the current page.
4. When they say yes:
   - Level 1: first move the current docs/ folder into set-aside/NN-before-goback (the next free number; make set-aside/ and that folder first if they aren't there yet). Moving and copying back both need a terminal command (mv and cp -R, or Move-Item and Copy-Item -Recurse on Windows), so say so before each permission request. Moving isn't deleting: everything is still there in set-aside/. Then copy that version's docs/ back into the project with one copy command (cp -R, or Copy-Item -Recurse on Windows), so pictures come back too and the page matches the save exactly. Never delete anything.
   - Level 2: make a new save that puts docs/ back exactly the way it was in that version, including taking out files that version didn't have (for example with git restore --source=<that save> --staged --worktree -- docs). History keeps everything; nothing is rewritten.
5. Add a line to NOTES.md saying which version you restored and why.
6. Ask them to look at the page and confirm it's how they remember it. Then, in one or two sentences, explain what probably went wrong in the version they left behind.
