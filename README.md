# NEXON Whitepaper

Source of truth for the NEXON whitepaper, in English and Simplified Chinese.
Published through GitBook via Git Sync — **this file is not part of the published site.**

## Layout

```
gitbook-docs.yaml     site-level mapping (sections, spaces, languages)
docs/en/              English space   → .gitbook.yaml · README.md · SUMMARY.md
docs/zh/              Chinese space   → .gitbook.yaml · README.md · SUMMARY.md
```

The two trees use identical file paths, so every chapter has a 1:1 counterpart.
Adding a chapter means adding it to **both** trees and to **both** `SUMMARY.md` files.

## Working rules

1. **Git Sync is bi-directional.** Edit either in the repo or in the GitBook editor — never
   both at once, or you will get conflicting commits. After the first sync, `git pull`:
   GitBook normalises Markdown and will have rewritten files.
2. **`README.md` files are managed here, not in GitBook.** Editing them in the GitBook editor
   creates duplicate pages.
3. **Assets are not shared between spaces.** An image used in both languages needs a copy in
   `docs/en/.gitbook/assets/` *and* `docs/zh/.gitbook/assets/`.
4. **Never change a `key` in `gitbook-docs.yaml`.** See the warning in that file.
5. **Terminology is fixed.** Both languages follow the locked four-layer term system; the
   Chinese is the source and the English must not drift from the agreed pairings.
