# Learnings

Short lessons from past sessions that change how we work. Newest first.

Claude loads this file at the start of every session, and `/close-out` adds to it at the end.
Keep it short, about ten entries at most. When a learning becomes a rule in `CLAUDE.md` or a step in a skill, delete it from here.

## Entry format

```
## YYYY-MM-DD: The lesson in one line

- What happened: one sentence
- Next time: what to do differently
```

---

## 2026-11-12: Create the GitHub repo before asking Claude to push

- What happened: A Claude Code cloud session could push to repos that already exist, but it was not allowed to create a new one, so the push waited on the founder.
- Next time: Create an empty repo at github.com/new first (no README, no license), then give Claude the link.

## 2026-11-12: Review with fresh eyes before the first commit

- What happened: Three reviewers (a beginner, a consistency checker, a fact checker) found 22 problems in the first draft of this repo that the writers had missed.
- Next time: For anything students or customers will read, have the reviewer agent check it before you commit.

## 2026-11-12: Check what a feature needs before teaching it

- What happened: The fact check found that ultracode workflows need a paid plan, and on the Pro plan must be turned on in `/config`. The first draft of lesson 4 did not say so.
- Next time: When a lesson depends on a Claude Code feature, check the official docs and state what the student needs up front.
