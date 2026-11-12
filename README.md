# Founder OS Starter

One repo that holds everything about your company, for you and your AI agents to share.

## What it is

Founder OS Starter is a small, ready to use folder structure for running a company with Claude Code. It stores what your company is, what you have decided, and what you have learned, as plain Markdown files. Claude loads the rules in `CLAUDE.md` at the start of every session and reads your company files before it writes anything about your business. Once you have taught it your company, you do not have to explain it again.

It is also a teaching repo. Five short lessons walk a beginner from a first prompt to running many agents at once.

New to the words? A repo is a folder whose history is tracked by a tool called git. Markdown is plain text with simple marks for headings and lists. Claude Code is Anthropic's AI tool that can read and change the files in a folder. A session is one conversation with Claude in that folder, a prompt is a message you type, and an agent is a helper Claude hands a job to.

## Description

Most people start every AI conversation from zero. They explain the business again, paste the same facts again, and lose the good answers when the chat closes. Founder OS fixes that by putting the context in one place that both people and agents can read.

It has six parts. Each one has one job.

| Element | Where | Its job |
| --- | --- | --- |
| Rules | [`CLAUDE.md`](CLAUDE.md) | Tells Claude how this repo works. Loaded at the start of every session. |
| Context | [`company/`](company/README.md) | The facts: who you are, who you serve, what you sell, how you sound. |
| Memory | [`history/`](history/README.md) | What happened, what you decided and why, and what you learned. |
| Work | `projects/`, `website/`, `apps/` | The things you build, each using the context. |
| Agents | `.claude/agents/` | Helpers with one job each: researcher, writer, reviewer. |
| Skills | `.claude/skills/` | Commands you type: `/onboard` to start, `/close-out` to finish. |

### Where things live

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

The starter comes filled in with a made up example company, Sunrise Dog Walking, so you have a working example to explore from the first minute. It is fictional. You replace it with your own company in lesson 2.

## The impact

What changes when your company lives in a repo like this:

- **You stop repeating yourself.** You teach Claude your company once. Every later session can read it from the files.
- **The work fits your business.** Website copy, emails and apps are written from your real facts and in your voice, not from guesses.
- **Less gets lost.** Decisions and the reasons behind them are written down, so you can find them months later.
- **Sessions build on each other.** When you run `/close-out`, it saves what was learned and makes small fixes to the repo itself, so the next session starts smarter.
- **Everything shares one source of truth.** The website, your agents and any future apps all read the same `company/` files. Change a price once and everything can follow.
- **You own it.** It is plain text in a folder you control. No special app is needed to read it, and git keeps the full history.

## How to get started

You need Claude Code and a GitHub account. To install Claude Code or sign in, follow the official docs at https://code.claude.com/docs.

1. **Get your own copy.** On this repo's GitHub page, click the green "Use this template" button to make your own copy, then clone it. Clone means download a copy that stays linked to GitHub. Not sure how, or no button? Open Claude Code in any folder and type: `Help me get this repo onto my computer and check that git is set up.` [Lesson 1](lessons/01-get-set-up.md) has more help.
2. **Open the `founder-os-starter` folder in the Claude Code desktop app** and start a new session.
3. **Type your first prompt:**

   ```
   Read CLAUDE.md and tell me what this repo is
   ```

4. **Follow the lessons in order.** Each one takes about 10 to 15 minutes.

   | Lesson | What you do |
   | --- | --- |
   | [1. Get set up](lessons/01-get-set-up.md) | Open the repo in Claude Code and try your first prompts |
   | [2. Teach it your company](lessons/02-teach-it-your-company.md) | Run `/onboard` and replace the example company with yours |
   | [3. Build the website](lessons/03-build-the-website.md) | Update the website from your company facts and preview it |
   | [4. Agents and ultracode](lessons/04-agents-and-ultracode.md) | Meet the three agents, then run many agents at once |
   | [5. Keep the history](lessons/05-keep-the-history.md) | Run `/close-out` so every session leaves the repo smarter |

## What to use

Pick the tool that fits the job.

| When you want to | Use | Example |
| --- | --- | --- |
| Set up your company for the first time | `/onboard` | Type `/onboard` and answer the 8 short questions Claude asks |
| Find something you wrote down | The researcher agent | `Use the researcher agent to find out what our goals are this year` |
| Get words written in your voice | The writer agent | `Use the writer agent to draft a welcome email for new customers` |
| Check work before you share it | The reviewer agent | `Use the reviewer agent to check the website against company/` |
| Change the website | A normal prompt | `Update website/index.html to match company/offerings.md` |
| Do a big job with many agents | Ultracode | `ultracode: write three versions of the intro in website/index.html, have reviewers check each against company/, then use the best one` |
| End a session | `/close-out` | Type `/close-out` and read the summary |

A note on ultracode: putting the word ultracode in a prompt tells Claude to split a big job across many agents at once. It uses many more tokens (the units of text Claude reads and writes, which count against your usage) than a normal prompt. It needs a paid Claude plan, and on the Pro plan you first turn on Dynamic workflows by typing `/config` in Claude Code. [Lesson 4](lessons/04-agents-and-ultracode.md) explains it.

## Best practices

1. **Keep `company/` true.** It is the source of truth. When a price, offer or goal changes, change it there first, then ask Claude to update everything that uses it.
2. **One topic per file, and keep files short.** Short files with clear headings are easier for people to scan and for agents to use.
3. **Write down the why.** A decision without a reason gets argued about again. Each entry in `history/decisions.md` has a date, the decision and why.
4. **Never let Claude guess a fact.** If something is missing, it should ask you, then save your answer in the right file. This is a house rule in `CLAUDE.md`.
5. **Start every project with a brief.** A short `brief.md` in `projects/` (goal, audience, what done looks like) gives much better results than a long chat.
6. **Review before you share.** Have the reviewer agent check anything customers will read.
7. **End every session with `/close-out`.** If it is not written down, the next session will not know it.
8. **Commit often.** A commit is a saved snapshot. Small, frequent commits make it easy to undo a mistake.
9. **Keep secrets out.** Never put passwords, API keys (secret codes that let software use a paid service) or private customer data in this repo, and take extra care if the repo is public.

## Tips

- **Ask where an answer came from.** Try `Which files did you read to answer that?` It shows you what Claude knows and what is missing.
- **Start a session by catching up.** Try `What did we do last session, and what should we do next?`
- **Correct Claude out loud.** When it gets something wrong, say so, then ask it to save the fix: `Add that to company/brand-voice.md so you remember it.`
- **Use the smallest tool that works.** A normal prompt for small edits, one agent for a focused job, ultracode for big or important work.
- **Add files as your company grows.** New topics get new files in `company/`, such as `faq.md`, `team.md` or `competitors.md`. Tell Claude about them in `CLAUDE.md`.
- **Read `history/learnings.md` now and then.** It is the list of lessons Claude follows. Delete any that no longer help.
- **Preview the website by opening it.** Double click `website/index.html`. There is nothing to install or build.
- **When stuck, ask Claude to explain.** Try `Explain what you just did in plain words.` This repo is made for learning.

## License

MIT. See [LICENSE](LICENSE). Copy it, change it, share it.
