---
name: onboard
description: Interviews the founder one question at a time, then replaces the example company in company/ with their real company. Run this once when setting up the repo, or again when the company changes a lot.
---

# Onboard

Replace the made up example company (Sunrise Dog Walking) with the
founder's real company.

## Steps

1. Read the four files in `company/` so you know the format to keep.
2. Tell the founder you will ask 8 short questions, one at a time.
3. Ask each question, then wait for the answer before asking the next.
   If an answer is unclear, ask one short follow up. If they say "skip",
   move on.
   1. What is the name of your company, who founded it, and when? Do
      you have a tagline?
   2. What do you do, in one or two sentences, and what is your mission?
   3. Who do you serve?
   4. What is the main problem they have?
   5. What do you offer, and what does each thing cost?
   6. How do you want to sound? Any words you like or want to avoid?
   7. What are your goals for this year?
   8. How can customers contact you, and where do you work?
4. Rewrite these files with the real answers. Keep the same headings and
   keep each file short:
   - `company/overview.md` (questions 1, 2, 7, 8)
   - `company/customers.md` (questions 3, 4)
   - `company/offerings.md` (question 5)
   - `company/brand-voice.md` (question 6)
5. Use the founder's own words where you can. Do not invent facts. Where
   a question was skipped, or a field in a file has no answer (for
   example founder, founded year, tagline, or mission), write
   "TODO: not answered yet".
6. Remove every mention of the example company and its founder from
   those four files.
7. Add an entry at the top of `history/decisions.md` with today's date:
   the decision (replaced the example company with the real one) and why.
8. Show a short summary: the files you changed, the main facts in each,
   and any TODO items left. Mention that the website still describes the
   example company, and that lesson 3 covers updating it.
