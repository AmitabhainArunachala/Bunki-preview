# Bunki-preview

Phone previews of **Bunki / KAIRO** release candidates. **This is not the product.** The live app is
[AmitabhainArunachala/Bunki-app](https://github.com/AmitabhainArunachala/Bunki-app), published at
https://amitabhainarunachala.github.io/Bunki-app/ by its own release workflow.

The `preview` workflow builds any Bunki-app branch, tag or commit with the production builder
(`scripts/build-corridor-site.mjs`) and publishes it here:

- Preview address: https://amitabhainarunachala.github.io/Bunki-preview/
- What is on it: https://amitabhainarunachala.github.io/Bunki-preview/preview.json (ref, commit, note, build time)

One preview is live at a time; each run replaces the last. Nothing here ever deploys to the live app.

Run one:

```sh
gh workflow run preview.yml -R AmitabhainArunachala/Bunki-preview -f ref=<branch-or-sha> -f note="<what this is>"
```
