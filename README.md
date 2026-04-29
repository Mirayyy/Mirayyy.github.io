# Mirayyy.github.io

This repository is a GitHub Pages user site that redirects all root-domain traffic to the project site at `/DeltaOps/`.

How it works:
- `index.html` redirects requests from `/` and existing root-level pages to `/DeltaOps/...`.
- `404.html` redirects unknown root-domain paths to `/DeltaOps/...`.
- The redirect keeps the original path, query string, and hash.
- URLs that already start with `/DeltaOps/` are not redirected again.

Example:
- `/stats?tab=top#main` becomes `/DeltaOps/stats?tab=top#main`
