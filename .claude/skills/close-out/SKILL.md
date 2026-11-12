---
name: close-out
description: Closes out a working session. Saves a session note, logs decisions, records what was learned, makes small improvements to this repo, then commits and pushes. Run this at the end of every session so the next one starts smarter.
---

# Close out

End the session so that nothing is lost and the repo gets a little
better each time. Do the steps in order. Keep everything short.

## Steps

1. Look back over this conversation. Work out what was done, what was
   decided, what went wrong or took too long, and where the founder
   corrected you.
2. Save a session note. Create `history/sessions/YYYY-MM-DD-topic.md`
   with today's date and a short topic in lowercase words joined by
   hyphens. If the file exists, add to it. Use these headings, a few
   bullets each, and name the files that changed:
   - What we did
   - What we learned
   - Decisions (only if any were made)
   - Next steps
3. Log decisions. Add each one at the top of `history/decisions.md` in
   the format shown there. Only log decisions the founder actually made.
   If you are not sure, ask.
4. Learn. Add up to three entries at the top of `history/learnings.md`
   in the format shown there. A learning is worth saving only if it
   would change what you do in a future session. Corrections from the
   founder come first. If there is nothing new, add nothing. Keep the
   file to about ten entries. If it is longer, merge similar ones or
   delete the least useful, and say which in the summary.
5. Improve. Use the learnings to make the repo itself better, with one
   or two small changes at most. Good places to improve:
   - `CLAUDE.md`: add or sharpen a house rule
   - `.claude/skills/` and `.claude/agents/`: fix a step or instruction
     that caused trouble
   - `company/`: fill in a fact the founder gave you during the session
   - `history/learnings.md`: remove a learning once it has become a rule
     somewhere else, so the list stays short
   Make small changes right away. Ask first before you delete a file,
   change or remove an existing house rule, change a company fact you
   are unsure of, or make a big change. Keep `CLAUDE.md` short: if you
   add a rule, check whether it can merge with one already there.
6. Show a short summary with four parts: Saved (the note and decisions),
   Learned, Improved (each change and why), and Start here next time
   (the first next step). List the files that will be committed. Ask if
   anything is missing or wrong, and fix it.
7. Once the founder says yes, commit with a clear message, then push.
   If there is no GitHub copy to push to, say so and stop after the
   commit.
