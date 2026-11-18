---
name: wrapup
description: End the session: notes, scorecard, recall questions, build review.
disable-model-invocation: true
---

1. Update "Current status" and add 1 to "Session number" in CLAUDE.md. Add a NOTES line for today.
2. Add this session's line under "By session" in HABITS.md, in the format shown there.
3. Ask three quick questions, one at a time, and give friendly feedback on each answer:
   - "If the next thing you build breaks everything, what would you do?"
   - "Why do we make a plan before building?"
   - "What's one idea you parked under 'Not in version 1'?"
4. Write the build review to reviews/session-NN.md using the format below. If there's no reviews/ folder yet, this is the first review: writing the file makes the folder. Tag 5 to 10 moves, in the order they happened. Every ?!, ? and ?? gets a "Better:" line. Use only moves that actually happened this session.
5. Show them the review in plain words: the best move, the one to work on, and the counts.
6. Tell them how to pick up next time: /pickup.
7. At level 2: if there are saved changes that aren't merged, remind them once (/ship).

Tags:
!! Brilliant: a habit done on their own at the moment it mattered most.
! Great: a great prompt (one step, clear, says what done looks like) or a save on their own.
✓ Good: the right habit, after a reminder.
?! Inaccuracy: a vague ask, or approving without reading.
? Mistake: a missed plan, or several working changes with no save.
?? Blunder: building on top of something unchecked, merging without reading the change, putting something private in a file.

Format:
# Build review: session NN (date, computer or phone)
Project: ... Level: 1 runs on my computer / 2 live at <link>
Result: one line on what works now
Moves: x brilliant, x great, x good, x inaccuracies, x mistakes, x blunders

1. [tag] [name of the move]. What happened, one line. Better: (for ?!, ?, ??)

Best move: #n
Work on next time: one habit, one line
Recall: their answers in one line each
