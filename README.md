# TheoTown Plugin Hub

A free static site (GitHub Pages) with a plugin library, forum boards and plugin submissions.

## Setup (works from a phone browser)
1. Create a public repo named `theotown-hub`. Upload `index.html`, `plugins.json`, `README.md`. Use Add file > Create new file to make `.github/ISSUE_TEMPLATE/submit-plugin.yml` and paste its content.
2. Open index.html, edit the line `REPO:"YOURNAME/theotown-hub"` to your real username/repo. Also replace YOURNAME in plugins.json.
3. Settings > Pages > Deploy from branch > main > Save. Your site: `https://YOURNAME.github.io/theotown-hub`.
4. Forum: Settings > General > enable Discussions. Install the giscus app (github.com/apps/giscus) on the repo. Open giscus.app, enter your repo, pick a Discussions category, then copy `data-repo-id` and `data-category-id` into the `CFG` block in index.html.
5. Plugin files: Releases > Draft new release > attach your zip. Put that release link in `download` in plugins.json.

## Adding plugins
Visitors use the Submit tab (opens an issue form). You review, then add the entry to plugins.json.

## Limits
Static site: no accounts or uploads of its own. Logins, comments and threads use GitHub accounts (giscus and Discussions).
