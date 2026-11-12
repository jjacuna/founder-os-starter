# Lesson 2: Teach it your company

## Goal

Replace the example company with your own, so Claude knows your business.

## Steps

1. Look at what is there now. Open the [company](../company/README.md)
   folder and read the four short files. They describe Sunrise Dog
   Walking, a made up example.

2. No company yet? Skip `/onboard`, keep the example, and go to step 5.
   Otherwise, run the onboard skill. A skill is a saved set of
   instructions that you start by typing a slash and its name.

   ```
   /onboard
   ```

3. Answer the questions. Claude asks about 8 of them, one at a time: your
   company name and founder, what you do, who you serve, their main problem, what you offer
   and the prices, how you sound, your goals, and your contact details.
   Short answers are fine. Say "skip" if you do not know yet.

4. Read the summary Claude shows at the end. It lists the files it
   rewrote. Claude may ask for permission before it changes a file. Read
   what it wants to change, then allow it.

5. Review the files yourself. Open each one and check that it is true:
   - [company/overview.md](../company/overview.md)
   - [company/customers.md](../company/customers.md)
   - [company/offerings.md](../company/offerings.md)
   - [company/brand-voice.md](../company/brand-voice.md)

6. Fix anything that is wrong. You can edit the file by hand, or ask:

   ```
   In company/offerings.md, change the price of the first item to $40.
   ```

7. Test it. Start a new session and ask a question only your files can
   answer.

   ```
   Who are our customers and what problem do we solve for them?
   ```

## What you learned

- Context is what Claude knows about you. It comes from these files, not
  from memory of past chats.
- One topic per file keeps facts easy to find and easy to fix.
- When a fact changes, change it in `company/` first. Everything else is
  built from there.

## Next

[Lesson 3: Build the website](03-build-the-website.md)
