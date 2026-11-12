# Lesson 5: Keep the history

## Goal

End every session by saving what you did and decided, so nothing is lost.

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

   These are examples for the made up company. Once you have your own
   first note, delete the example session note and the two example
   decisions.

3. Run the log session skill at the end of your work.

   ```
   /log-session
   ```

4. Read what Claude wrote. It creates a new note in `history/sessions/`
   named with today's date and a topic, and adds any decisions to the
   decision log. Correct anything that is wrong.

5. Add a decision yourself if one is missing.

   ```
   Add a decision to history/decisions.md: we will post a weekly update
   on the website, because clients asked for news.
   ```

6. Commit, so the history is saved with the work. Then push, which
   sends your saved snapshots to your copy on GitHub.

   ```
   Commit these changes with a clear message, then push to GitHub
   ```

7. Test the memory. Start a new session and ask:

   ```
   What did we do last session, and what should we do next?
   ```

## What you learned

- The repo is the memory. If it is not written down, the next session
  will not know it.
- The decision log records why, which is the part people forget first.
- The habit: finish work, run `/log-session`, commit.

## Next

You have finished the lessons. Go back to the [README](../README.md) and
start your next project in [projects](../projects/README.md). When you are
ready to build an app, see [apps](../apps/README.md).
