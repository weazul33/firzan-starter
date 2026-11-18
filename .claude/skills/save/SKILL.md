---
name: save
description: Save a version of the project after a step works.
disable-model-invocation: true
---

Read "Where it lives" in CLAUDE.md first.

At level 1 (my computer):
Use your own file tools to read and write the files, not terminal commands, so this works the same on every computer. Don't use git.
1. Look in versions/ and pick the next number: 01, 02, 03 and so on. If there's no versions/ folder yet, this is the first save: the number is 01, and the folder gets made when you copy the files in step 3.
2. Ask for a two- or three-word label, or suggest one. The new folder is versions/NN-label, for example versions/03-added-photos.
3. Copy every project file into it, keeping the same folder layout. Skip versions/, set-aside/, reviews/ and .claude/.

At level 2 (GitHub):
1. Ask for a two- or three-word label, or suggest one.
2. Make a commit with that label on this session's branch and push it. Never force-push, never push to main.
3. Say: "Saved on GitHub, not live yet. /ship puts it live."

At both levels:
4. Add one line to the log in NOTES.md: the label and what works now.
5. Update HABITS.md: count habit 6 under "On my own" if they typed /save without you suggesting it in your last reply, otherwise under "Reminded."
6. Tell them in one line what was saved and that /goback can bring it back any time.
