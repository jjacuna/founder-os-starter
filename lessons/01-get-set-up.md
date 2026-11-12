# Lesson 1: Get set up

## Goal

Open this repo in Claude Code and ask it your first questions.

## Steps

1. Install Claude Code and sign in. Follow the official docs at
   <https://code.claude.com/docs>. Claude Code comes as a desktop app
   (Mac and Windows, with Linux in beta), a terminal tool, a web app at claude.ai/code, and
   editor extensions. These lessons use the desktop app.

2. Get a copy of this repo onto your computer. A repo (short for
   repository) is a folder whose history is tracked by a tool called git.
   On the repo's GitHub page, click "Use this template" to make your own
   copy, then clone it. Clone means download a copy that stays linked to
   GitHub. Not sure how? Open Claude Code in any folder and ask:

   ```
   Help me get this repo onto my computer and check that git is set up.
   ```

3. Open the `founder-os-starter` folder in the Claude Code desktop app
   and start a new session. A session is one conversation with Claude
   inside this folder.

4. Type your first prompt. A prompt is just a message to Claude.

   ```
   What is this repo for? Give me a short tour of the folders.
   ```

5. Ask about the example company. Claude answers by reading the files in
   `company/`.

   ```
   What does Sunrise Dog Walking offer, and what does each service cost?
   ```

6. Ask how Claude knew where to look.

   ```
   Which files did you read to answer that?
   ```

7. Open [CLAUDE.md](../CLAUDE.md) and read it. Claude Code loads this
   file by itself at the start of every session in this folder. It is how
   Claude knows the house rules before you say a word.

   Markdown is plain text with a few simple marks, like `#` for a heading.
   A `.md` file opens in any text editor. Or just ask Claude:
   `Show me CLAUDE.md`

## What you learned

- A repo is a folder with a tracked history. This one holds your company's
  context in plain Markdown files.
- Claude reads the files in the folder to answer you. Better files mean
  better answers.
- `CLAUDE.md` is loaded at the start of every session, so it is the place
  for instructions Claude should always follow.

## Next

[Lesson 2: Teach it your company](02-teach-it-your-company.md)
