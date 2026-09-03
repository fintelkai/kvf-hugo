# kvf-site — Hugo blog (*semantics etc.*)

Hugo source for the *semantics etc.* blog. Posts in `content/post/`, theme via `layouts/`, build with `hugo`.

## New posts

`content/post/<slug>.md`. The filename becomes the URL via `[permalinks] post = "/:slug/"` in `config.toml`.

Modern frontmatter — used by every post since 2021 — is just:

```
---
title: "Post Title"
date: 2026-06-03
draft: false
---
```

No `tags`, no `url`. Older posts (pre-2021) use a different shape with tag lists and explicit `url:` fields; don't copy that pattern for new posts.

Body is plain markdown; `markup.goldmark.renderer.unsafe = true` is on, so raw HTML works.

## Local preview

`hugo server` from this directory. Port 1313 is usually already in use by the `g-lifelist` Hugo server at `~/Documents/photoproject/g-lifelist/hugo/` — pass `--port 1314` to avoid the conflict.

## Pushing

Never `git push` without an explicit ask in the current turn — the `~/Documents/CLAUDE.md` rule, in full force here. Stage and commit freely; the push is a separate, asked-for step.

When asked, it works: the HTTPS remote has a working credential helper, verified 2026-09-03 with a non-interactive push. This section used to say there were no cached credentials and that the push had to be handed back; that was wrong, and it made a standing instruction look like a technical limit.

## Build artifacts

`/public/` and `.hugo_build.lock` are git-ignored (added 2026-06). Don't commit them.
