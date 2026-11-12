# history/

This folder is the memory of the company: what happened, and why.

## What goes here

- [decisions.md](decisions.md): the decision log. One short entry per decision, newest first.
- [sessions/](sessions/): one note per work session. See the example,
  [2026-11-12-first-session.md](sessions/2026-11-12-first-session.md).

## How agents use it

A new Claude session does not remember the last one.
Agents read this folder to learn what was already done and why, so they do not redo work or undo a choice.

## How to add to it

- Run `/log-session` at the end of a work session. It writes a session note and adds any decisions to the log.
- Name session notes `YYYY-MM-DD-topic.md`, for example `2026-11-12-first-session.md`.
- Do not rewrite old entries. If a decision changes, add a new entry that says so.
