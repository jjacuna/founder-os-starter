# CLAUDE.md

Claude Code loads this file at the start of every session in this folder.

## What this repo is

This is a Founder OS: one repo that holds everything about one company in plain Markdown. You read it to learn the company, then use that context to help build the website and, later, apps. The people using it are often new to Claude Code and to git, so explain what you are doing in plain words.

The repo starts with a made up example company, Sunrise Dog Walking. Once the founder runs `/onboard`, the files describe their real company.

## Where things live

- `company/`: the facts. Overview, customers, offerings, brand voice. One topic per file.
- `history/decisions.md`: the decision log, newest first.
- `history/sessions/`: one short note per work session.
- `history/learnings.md`: lessons from past sessions that change how we work.
- `projects/`: one subfolder per project, each with a `brief.md`.
- `website/`: the one page site (`index.html` and `styles.css`).
- `apps/`: future apps, each in its own folder.
- `lessons/`: the teaching guide for students.
- `.claude/agents/`: three subagents: researcher, writer, reviewer.
- `.claude/skills/`: two skills: `/onboard` and `/close-out`.

## Start of every session

1. Follow the learnings from past sessions. They are loaded here automatically: @history/learnings.md
2. Read the note in `history/sessions/` with the latest date in its name, so you know where things stopped. If several share that date, read them all. Skip `2026-11-12-first-session.md`, it is an example.

## House rules

1. Read the files in `company/` before you write anything about the company.
2. Never invent company facts (names, prices, dates, numbers, claims). If a fact is missing, ask the founder, then save the answer in the right `company/` file.
3. Write in the voice described in `company/brand-voice.md`.
4. Keep files short and simple. Plain words. A beginner should understand a file in one read.
5. The website is plain HTML and CSS with no build step. Do not add frameworks, packages or build tools.
6. When a decision is made, add it to the top of `history/decisions.md` with the date, the decision and why.
7. At the end of a work session, offer to run `/close-out`. It saves the session, records what was learned, and improves this repo.
8. Never use em dashes or en dashes. Use commas, periods, colons or parentheses.
9. Before starting a project, read its `brief.md` in `projects/`.
