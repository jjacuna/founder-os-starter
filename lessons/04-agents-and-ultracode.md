# Lesson 4: Agents and ultracode

## Goal

Use a single helper agent, then run many agents at once with ultracode.

## Steps

1. Learn what a subagent is. It is a helper with one job and its own
   instructions. Each one is a Markdown file in `.claude/agents/`. Claude
   hands work to a subagent when the task matches its description, or
   when you ask for it by name. This repo has three:
   - [researcher](../.claude/agents/researcher.md): answers questions
     from the library and names its sources. It cannot change files.
   - [writer](../.claude/agents/writer.md): drafts copy in your brand
     voice.
   - [reviewer](../.claude/agents/reviewer.md): checks work against your
     facts and reports problems. It cannot change files.

2. Open one of those files. The top part says when Claude should use the
   agent and what it may do. The rest is its instructions.

3. Ask for an agent by name.

   ```
   Use the researcher agent to find out what our goals are this year.
   ```

A caution on cost before the next step: ultracode uses many more tokens
than a normal prompt. Tokens are the units of text Claude reads and
writes, and your usage is measured in them. Use ultracode for big or
important jobs, not small edits. Short on usage? Read step 4 and skip
running it.

4. Now try ultracode. Putting the word "ultracode" in a prompt tells
   Claude to plan a workflow: it writes a small script that sends the
   work to many agents at once. You can also say "use a workflow".

   ```
   ultracode: write three different versions of the intro section of website/index.html, have reviewers check each against company/, then use the best one
   ```

   Workflows need a paid Claude plan. On the Pro plan, first turn on
   Dynamic workflows in `/config`. If your organization has turned
   workflows off, this exercise will not run.

5. Watch what happens. Claude shows the planned phases and asks you to
   approve the run (the desktop app offers Once, Always, or Deny). Watch
   progress in the Background tasks pane. In a terminal session you can
   also type `/workflows`.

6. When it finishes, read the summary and refresh the website.

## What you learned

- A subagent is a Markdown file that gives Claude a focused helper.
- Ultracode runs many agents in parallel and has them check each other.
- More agents cost more tokens. Pick the smallest tool that does the job.

## Next

[Lesson 5: Keep the history](05-keep-the-history.md)
