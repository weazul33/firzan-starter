---
name: save
description: Save a version of the project after a step works.
disable-model-invocation: true
---

Read "Where it lives" in CLAUDE.md first. If it starts with "GitHub:", this is level 2: skip every level 1 step and don't make a versions/ folder, even if NOTES.md or an older review mentions versions. Otherwise it's level 1.

At level 1 (my computer):
Copy with one terminal command that copies whole folders (cp -R on a Mac, Copy-Item -Recurse on Windows), because your file tools can't copy pictures. Say in one sentence what the command does before the permission request. Don't use git.
1. Look in versions/ and pick the next number: 01, 02, 03 and so on. If there's no versions/ folder yet, this is the first save: the number is 01. Don't make any folder yet.
2. If they typed a label with the command (for example "/save added photos"), use it. Otherwise ask for a two- or three-word label, or suggest one, and wait for their answer before copying anything. The new folder is versions/NN-label, for example versions/03-added-photos.
3. Once the label is agreed, make versions/NN-label and copy every project file into it, keeping the same folder layout, in one command line (for example mkdir and cp -R joined with &&, or New-Item and Copy-Item -Recurse on Windows). That's one permission box. Skip versions/, set-aside/, reviews/ and .claude/.

At level 2 (GitHub):
1. If they typed a label with the command, use it. Otherwise ask for a two- or three-word label, or suggest one, and wait for their answer.
2. Before you commit, do steps 4 and 5 below now (not again later), so the log line and the habit count go into the same commit. Then look at every file that changed (not just docs/) for anything private, like a phone number or home address. Their project is public, so a push can be seen right away, even before /ship. Fix it with them first. Then make a commit with that label on this session's branch and push it. Never force-push, never push to main.
3. Say: "Saved on GitHub, not live yet. /ship puts it live."

At both levels:
4. Add one line to the log in NOTES.md: the label and what works now.
5. Update HABITS.md: count habit 6 under "On my own" if they typed /save without you suggesting it in your last reply, otherwise under "Reminded."
6. Tell them in one line what was saved and that /goback can bring it back any time.
