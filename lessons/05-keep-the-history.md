# Lesson 5: Keep the history

## Goal

End every session with `/close-out`, so nothing is lost and the repo gets
a little better each time.

## Steps

1. Understand the problem. Claude does not carry a conversation into the
   next session. What it knows next time is what is written in this repo.
   So before you stop, write things down.

2. Look at the examples already here:
   - [history/decisions.md](../history/decisions.md) is the decision log.
     Newest first. Each entry has a date, the decision, and why.
   - [history/sessions/2026-11-12-first-session.md](../history/sessions/2026-11-12-first-session.md)
     is a session note: what we did, what we learned, decisions (if
     any), and next steps.
   - [history/learnings.md](../history/learnings.md) is the list of
     lessons that change how you and Claude work. Claude reads it at the
     start of every session.

   These came with the starter. Once you have your own first note,
   delete the two session notes that came with the repo and the
   decisions that are not yours. Keep any learnings that still help you.

3. Run the close out skill at the end of your work.

   ```
   /close-out
   ```

4. Read the summary Claude shows. It has four parts:
   - Saved: a new note in `history/sessions/` and any decisions.
   - Learned: new entries in `history/learnings.md`.
   - Improved: one or two small fixes to the repo itself, such as a
     sharper rule in `CLAUDE.md`.
   - Start here next time: the first next step.

   Correct anything that is wrong, then say yes. Claude commits the
   work, which saves a snapshot, and pushes it to your copy on GitHub.

5. Add a decision yourself if one is missing.

   ```
   Add a decision to history/decisions.md: we will post a weekly update
   on the website, because clients asked for news. Then commit and push.
   ```

6. Test the memory. Start a new session and ask:

   ```
   What did we do last session, and what should we do next?
   ```

## What you learned

- The repo is the memory. If it is not written down, the next session
  will not know it.
- The decision log records why, which is the part people forget first.
- Learnings turn mistakes into rules, so the same problem does not
  come back.
- The habit: finish work, run `/close-out`.

## Next

You have finished the lessons. Go back to the [README](../README.md) and
start your next project in [projects](../projects/README.md). When you are
ready to build an app, see [apps](../apps/README.md).
