# Founder OS Starter

One repo that works as your company's brain. The facts about your company live in `company/`. The memory of what happened and why lives in `history/`. The work itself lives in `projects/`, `website/` and `apps/`. Everything is plain Markdown, so both you and AI agents like Claude Code can read it. When Claude knows your company, it can help you build things that fit it.

This starter comes filled in with a made up example company, Sunrise Dog Walking. It is fictional. You replace it with your own company in lesson 2.

## Quick start

1. Get your own copy. On the repo's GitHub page, click "Use this template" to make your own copy, then clone it. Clone means download a copy that stays linked to GitHub. [Lesson 1](lessons/01-get-set-up.md) has more help.
2. Open the folder in Claude Code. If you still need to install it or sign in, see the official docs at https://code.claude.com/docs.
3. Type this first prompt: `Read CLAUDE.md and tell me what this repo is`
4. Follow the lessons in [lessons/](lessons/README.md), in order. You will run `/onboard` in lesson 2 to replace the example company with your own.

## Folder map

```
founder-os-starter/
  README.md        # you are here
  CLAUDE.md        # instructions Claude reads at the start of every session
  company/         # the facts about the company, one topic per file
    overview.md      # what the company is, mission, goals
    customers.md     # who the customers are and their problems
    offerings.md     # products or services with prices
    brand-voice.md   # how the company sounds
  history/         # the memory of what happened and why
    decisions.md     # decision log, newest first
    learnings.md     # lessons that make each session better
    sessions/        # one short note per work session
  projects/        # one subfolder per project, each with a brief.md
    website/         # the brief for the starter website
  website/         # a one page site in plain HTML and CSS
  apps/            # future apps live here, each in its own folder
  lessons/         # five short lessons, start here to learn
  .claude/         # extras for Claude Code
    agents/          # three helper agents: researcher, writer, reviewer
    skills/          # two commands: /onboard and /close-out
  LICENSE          # MIT license
  .gitignore       # files git should not track
```

## The elements

Founder OS has six parts. Each one has one job.

| Element | Where | Its job |
| --- | --- | --- |
| Rules | `CLAUDE.md` | Tells Claude how this repo works. Loaded at the start of every session. |
| Context | `company/` | The facts: who you are, who you serve, what you sell, how you sound. |
| Memory | `history/` | What happened, what you decided and why, and what you learned. |
| Work | `projects/`, `website/`, `apps/` | The things you build, each using the context. |
| Agents | `.claude/agents/` | Helpers with one job each: researcher, writer, reviewer. |
| Skills | `.claude/skills/` | Commands you type: `/onboard` to start, `/close-out` to finish. |

## What you can use it for

- **Teach Claude your company once.** Run `/onboard`, and every later session already knows your facts and voice.
- **Build a website that matches your business.** The site in `website/` is written from the facts in `company/`.
- **Write on brand.** Ask the writer agent for emails, posts or page copy, and the reviewer agent to check them.
- **Find answers fast.** Ask the researcher agent what you decided, and why, months later.
- **Keep one source of truth for apps.** Every app in `apps/` reads the same `company/` files.
- **Learn agents and ultracode.** The lessons take you from one prompt to many agents working at once.
- **Get better every session.** `/close-out` saves what you learned and improves the repo itself.

## How it works

Claude Code reads [CLAUDE.md](CLAUDE.md) at the start of every session, so it always knows how this repo is laid out and what the house rules are. Before it writes anything about your company, it reads the files in [company/](company/README.md), so the work matches your real facts and your voice. At the end of a session, you run `/close-out`. It saves what you did and decided into [history/](history/README.md), writes down what was learned, and makes small improvements to the repo itself. Next time, Claude reads those learnings first, so every session starts a little smarter than the last.

## Learn it step by step

Start with the [lessons](lessons/README.md):

1. [Get set up](lessons/01-get-set-up.md)
2. [Teach it your company](lessons/02-teach-it-your-company.md)
3. [Build the website](lessons/03-build-the-website.md)
4. [Agents and ultracode](lessons/04-agents-and-ultracode.md)
5. [Keep the history](lessons/05-keep-the-history.md)

## License

MIT. See [LICENSE](LICENSE). Copy it, change it, share it.
