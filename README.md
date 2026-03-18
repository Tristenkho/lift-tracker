# lift-tracker

Static workout tracker deployed from GitHub Pages.

## Daily workflow

Edit the app locally in this repo, then publish with git:

```bash
git status
git add index.html README.md
git commit -m "Describe the change"
git push
```

After the push finishes, GitHub Pages deploys automatically from `main`.
Open the Pages URL on your phone and refresh.

## First-time setup

Point `origin` at the real GitHub repo:

```bash
git remote set-url origin https://github.com/<your-username>/lift-tracker.git
git push -u origin main
```

Then enable GitHub Pages:

1. Open the repo on GitHub.
2. Go to `Settings` -> `Pages`.
3. Under `Build and deployment`, choose `Deploy from a branch`.
4. Select branch `main` and folder `/ (root)`.

Your phone URL will be:

```text
https://<your-username>.github.io/lift-tracker/
```

## AI workflow

Do not replace the whole file in GitHub by copy-pasting.
Let AI edit the local repo, then review the diff before pushing:

```bash
git diff -- index.html
```

This keeps changes small, reviewable, and reversible.

## Known gotchas

- If your iPhone home screen app looks stale, refresh or fully close and reopen it.
- GitHub Pages deploys are not instant. Wait 10-60 seconds after push.
- If `git push` fails, check both the remote URL and your GitHub auth.
