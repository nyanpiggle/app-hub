# Agent guide

`AGENTS.md` and `CLAUDE.md` are the same document. Read this before editing.

## Phone list (all nyanpiggle projects)

The home screen is <https://nyanpiggle.github.io/app-hub/>, this repo. It lists public repos that are not forks. `app-hub` itself is not a card. Private repos never appear.

A card opens, in order:

1. the repo Homepage / website URL, if one is set
2. otherwise `https://nyanpiggle.github.io/<repo>/` when GitHub Pages is on
3. otherwise the GitHub repo, which is the source, not the app

A change to an app is not finished when its source branch moves. The same turn must update the URL that card opens, then confirm the live page is the new one. Do not clear Homepage, turn Pages off, or make the repo private if it should stay on the phone. Repos do not all publish the same way. Copy this phone section into `AGENTS.md` and `CLAUDE.md` on any new project, then add how that repo publishes.

## This repo is the list

Pages serves `main` at the repo root, so a push to `main` updates every phone: <https://nyanpiggle.github.io/app-hub/>. There is no `gh-pages` branch. Do not add one. Do not force-push `main`.

`index.html` is the link order above (`homepage`, then Pages, then the repo). Keep that order. The name `app-hub` is skipped, so this repo is not its own card.

`.github/workflows/pages.yml` also deploys the repo root on a push to `main`. The phone update is still that push. Confirm <https://nyanpiggle.github.io/app-hub/> shows the change before you say it is done.
