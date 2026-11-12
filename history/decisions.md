# Decision log

A short record of choices we made and why. Newest first.

The entries below are for the made up example company. Keep them as a model, or delete them when you start your own log.

## Entry format

Copy this for each new decision and add it above the older entries:

```
## YYYY-MM-DD: The decision in one line

- Decision: what we chose
- Why: the reason, in a sentence or two
```

You can also run `/log-session` and Claude will add entries for you.

---

## 2026-11-12: Keep the website plain HTML and CSS

- Decision: The website is plain HTML and CSS with no build step. The files live in [website/](../website/).
- Why: Anyone can open the files and edit them. There is nothing to install and nothing to break.

## 2026-11-12: Start this repo as the single home for company context

- Decision: All company facts, history, and projects live in this one repo as Markdown files.
- Why: People and AI agents can read the same source. Nothing gets lost in chat windows or scattered documents.
