# Lesson 3: Build the website

## Goal

Update the one page website from your company facts, preview it, and save
your work with a commit.

## Steps

1. Preview the site as it is now. Open the `founder-os-starter` folder in
   Finder (Mac) or File Explorer (Windows), go into `website`, and double
   click `index.html`. It opens in your web browser. There is nothing to
   install, it is plain HTML and CSS.

2. Read the plan. Open [projects/website/brief.md](../projects/website/brief.md).
   A brief says what the project is for and when it is done. If you ran
   `/onboard`, ask Claude to bring the brief up to date first:

   ```
   Update projects/website/brief.md to match the facts in company/.
   ```

3. Ask Claude to update the site.

   ```
   Update website/index.html using the facts in company/ and the brief in
   projects/website/brief.md. Follow the brand voice. Do not invent facts.
   ```

4. Preview again. Go back to your browser and refresh the page.

5. Ask for changes in plain words until you like it. For example:

   ```
   Make the heading larger and move the prices section above the intro.
   ```

6. Check the facts. Compare the prices on the page with
   [company/offerings.md](../company/offerings.md) and the contact details
   with [company/overview.md](../company/overview.md).

7. Save your work with a commit. A commit is a saved snapshot of the repo
   with a short message that says what changed.

   ```
   Commit these changes with a clear message
   ```

   If Claude says git is not set up, ask it to set it up for this folder.

8. Back up and share your work. Push means send your saved snapshots to
   your copy on GitHub.

   ```
   Push my commits to GitHub
   ```

## What you learned

- The website is built from the facts in `company/`, so the site and the
  library stay in agreement.
- Work in small steps: ask, preview, adjust.
- A commit saves a snapshot you can always return to. Commit whenever
  something works.

## Next

[Lesson 4: Agents and ultracode](04-agents-and-ultracode.md)
