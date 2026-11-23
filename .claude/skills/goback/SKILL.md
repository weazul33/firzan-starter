---
name: goback
description: Put the page back to a saved version without deleting anything.
disable-model-invocation: true
---

Only the website (the docs folder) goes back. The brief, NOTES.md, HABITS.md and reviews/ stay as they are, so the scorecard and log keep counting.

1. Read "Where it lives" in CLAUDE.md. If it starts with "GitHub:", use only the level 2 steps: saves are commits, and versions/ isn't used. List the saved versions, newest first, in plain words: at level 1 the folders in versions/ with their NOTES line; at level 2 the recent saves (commits) on GitHub with their labels. At level 2, the save called "Add files via upload" is the version they put online at /level-up. Saves from versions/ on their computer didn't come along. At level 1, if there's no versions/ folder or it's empty, say plainly: nothing has been saved yet, so there's no version to go back to. Offer two ways out: type /rewind to undo my recent changes in this session, or we fix it together one small step at a time. Then stop this command.
2. Ask which one to go back to. Suggest the newest.
3. Before changing anything, compare the current docs/ with that version's docs/ file by file. Tell them in plain words what will come back and everything they'll lose from the current page, including changes that were never saved. At level 1, changes that were never saved leave the page, but they're kept in set-aside/ with everything else. At level 2, a change that was never saved is gone for good, so say that plainly and offer /save first.
4. When they say yes:
   - Level 1: first move the current docs/ folder into set-aside/NN-before-goback (the next free number; make set-aside/ and that folder first if they aren't there yet). Moving and copying back both need a terminal command (mv and cp -R, or Move-Item and Copy-Item -Recurse on Windows), so say so before each permission request. Moving isn't deleting: everything is still there in set-aside/. Then copy that version's docs/ back into the project with one copy command (cp -R, or Copy-Item -Recurse on Windows), so pictures come back too and the page matches the save exactly. Never delete anything.
   - Level 2: make a new save that puts docs/ back exactly the way it was in that version, including taking out files that version didn't have (for example with git restore --source=<that save> --staged --worktree -- docs). History keeps everything; nothing is rewritten. Before you commit, add the NOTES.md line from step 5 now (not again later), so it goes in the same commit. Check every changed file for anything private. Then commit with the label "back to <label>" and push it on this session's branch (never force, never to main). This isn't a /save: don't add a save line and don't count habit 6. Then say: "Saved on GitHub, not live yet. /ship puts it live."
5. Add a line to NOTES.md saying which version you restored and why. (At level 2 you already did this in step 4.)
6. For this session's HABITS line, count it as goback "own" if they typed /goback without you suggesting it in your reply just before, otherwise "reminded". Note it in your moves log.
7. Ask them to look at the page and confirm it's how they remember it (at level 2, on the live link once they've merged it with /ship). Then, in one or two sentences, explain what probably went wrong in the version they left behind.
