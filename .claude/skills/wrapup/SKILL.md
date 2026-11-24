---
name: wrapup
description: End the session: notes, scorecard, recall questions, build review.
disable-model-invocation: true
---

Before step 1, at level 2 only: get the latest from GitHub first (git fetch origin), then compare this branch with origin/main, not a local copy of main, which can be out of date. If docs/ has changes that aren't saved, or saved page changes that aren't merged yet, stop here. Suggest /save and /ship for them first, then come back to /wrapup (say that /wrapup ends with one more short /ship for the notes). That way the merge is counted before the review, and the wrap-up pull request has only notes. If they don't want them live, carry on, and say plainly: unsaved changes will be gone next time, and saved ones will be in the wrap-up pull request too.

1. At both levels: note the "Session number" in CLAUDE.md: that's this session's number. Use it below for the HABITS line, the review and the wrap-up label (session 1 is S1 and reviews/session-01.md). Then rewrite the whole of CLAUDE.md in one Write (its two parts are far apart): update "Current status" and add 1 to "Session number", ready for next time (keep using this session's number for the rest of this command). Read this session's notes under "Today" in NOTES.md, including any "counts so far" line, and keep them for steps 2 and 4. Then rewrite the whole of NOTES.md in one Write ("Today" sits between "Log" and "Words I've learned"): add a line for today under "Log", add every word you defined this session that isn't in "Words I've learned" yet, and clear this session's notes from "Today" (keep the heading and its line in brackets).
2. Add this session's line under "By session" in HABITS.md, in the format shown there. Include any "counts so far" line you kept from "Today" in step 1.
3. Ask three quick questions, one at a time, and give friendly feedback on each answer:
   - "If the next thing you build breaks everything, what would you do?"
   - "Why do we make a plan before building?"
   - "What's one idea you parked under 'Not in version 1'?"
   For the first question, accept any answer that means going back to the last save. Then add one line so it works outside this kit: in any Claude Code project, ask Claude to go back to your last saved version, or use /rewind to undo recent changes.
4. Write the build review to reviews/session-NN.md using the format below. If there's no reviews/ folder yet, this is the first review: writing the file makes the folder. Tag 5 to 10 moves, in the order they happened. Every ?!, ? and ?? gets a "Better:" line. Use your moves log and the "Today" notes you kept in step 1. Use only moves that actually happened this session, described only with what they said or did: don't add details they didn't give, such as which checks they tried or where a photo came from. At level 2, tag the merge from what they told you at /ship, not a guess.
5. Show them the review in plain words: the best move, the one to work on, and the counts.
6. Tell them how to pick up next time: /pickup. At level 1, add one line: your page only lives on this computer, so nobody else can see it yet. /level-up puts it online once version 1 works and is saved.
7. At level 2: what you just wrote (the brief, NOTES.md, HABITS.md and the review) is a change too, and right now it is only on this session's branch. Commit only CLAUDE.md, NOTES.md, HABITS.md and reviews/, not docs/. Commit them on this branch with the label "session NN wrap-up" and push, the same way /save does at level 2, but with no new log line: this doesn't count for habit 6. Then say: "Your notes and review only reach next time once they're merged. Type /ship once more. It makes a new pull request with just your notes and review, and it won't change your page." If they kept saved page changes back before step 1, say this pull request has those too, so it will change the page.

Tags:
!! Brilliant: a habit done on their own at the moment it mattered most.
! Great: a great prompt (one step, clear, says what done looks like), or a habit done on their own (a save, a check, a plan).
✓ Good: the right habit, after a reminder.
?! Inaccuracy: a vague ask, or approving without reading.
? Mistake: a missed plan, or two working changes piling up with no save.
?? Blunder: building on top of something unchecked, merging without reading the change, putting something private in a file.
A new idea outside "Done looks like" gets no tag on its own (parking it is the coach's job). Tag it only if the ask itself was vague (?!).

Format:
# Build review: session NN (date, computer or phone)
Project: ... Level: 1 runs on my computer / 2 live at <link>
Result: one line on what works now
Moves: x brilliant, x great, x good, x inaccuracies, x mistakes, x blunders

1. [tag] [name of the move]. What happened, one line. Better: (for ?!, ?, ??)

Best move: #n
Work on next time: one habit, one line
Recall: their answers in one line each
