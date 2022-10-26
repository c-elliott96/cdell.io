+++
title = "Homepage _index"
author = ["Christian Elliott"]
type = "homepage"
draft = true
+++

## Notes {#notes}


### Latex preview PNGs {#latex-preview-pngs}

My PNGs that are the LaTeX preview from ORG/\* are showing up in this
`cdell.io/static/ltximg` when I run `org-hugo-export-wim-to-md`.

Note: a temporary workaround for this dilemma is to .gitignore
`static/ltximg/*`, but this will likely interfere with embedded LaTeX in
Github Pages

The real concern here is committing content that is not intended for a
publicly facing repo, as Github Pages _must_ be.


### Known issues {#known-issues}

-   It looks like changing tags/categories will break a running server, locally.
-   Tags can't contain hyphens
    -   Can they be escaped?
