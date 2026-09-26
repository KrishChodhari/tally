# Tally — Business Calculator

A single-file, self-contained business/finance calculator, styled after the
Citizen SDC-868L. No build step, no dependencies to install — it's just
`index.html`.

**Features**
- Dual independent memories (M / M2), each with add, subtract, recall & clear
- MU (markup): cost → markup % → sell price
- `^` power key
- DEC switch: fix results to 0–3 decimal places, or leave unrounded (N)
- GRP switch: digit grouping — none (N), Indian 2-2-3 (IND), or international
  3-digit (INTL)
- On-screen backspace, keyboard input support
- Works on desktop and mobile browsers

## Deploy to GitHub Pages

1. **Create a new repository** on GitHub (public, so Pages can serve it for
   free). Don't initialize it with a README — you'll add this one.

2. **Upload the files.** Easiest way if you don't use git regularly:
   on the repo's GitHub page, click **Add file → Upload files**, drag in
   `index.html` and this `README.md`, then commit.

   Or, from the command line, in the folder containing these files:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Add Tally business calculator"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```

3. **Turn on Pages.** In the repo, go to **Settings → Pages**. Under
   "Build and deployment", set **Source** to **Deploy from a branch**, choose
   the **main** branch and the **/ (root)** folder, then **Save**.

4. **Wait a minute**, then refresh that Pages settings page — GitHub will
   show your live URL, something like:
   ```
   https://<your-username>.github.io/<your-repo>/
   ```

That's it — `index.html` at the repo root means the calculator loads directly
at that URL with no extra path.

## Making future changes

Edit `index.html` and push again (or re-upload it through the GitHub web UI).
GitHub Pages redeploys automatically within a minute or two of any push to
the branch it's watching.
