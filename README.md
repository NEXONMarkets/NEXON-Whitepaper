# NEXON Whitepaper

> ⚠️ **WORK IN PROGRESS — NOT AN OFFER.**
> The economic mechanism and worked examples reproduce the project party's approved
> 6 September 2026 Tokenomics paper. They are parameters and conditional illustrations,
> not promises of yield, price, payback or principal protection. Numerical EXON total supply,
> complete allocation and initial float remain unpublished. Participants may lose some or all principal.

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
5. **Narrative and mechanical roles are both fixed.** In the approved narrative, NEXON is
   the ecosystem, XO carries long-term value and EXON drives circulation. In the current
   economic mechanism, XO is the Staking Principal Token and EXON is the Core Value Token.
   Governance, payments, fees and consumption utilities remain Roadmap until their rules are
   published. Both languages must preserve this distinction and remain structurally aligned.
6. **Two linked sources of truth.** The economic source PDF is
   `../../../raw/NEXON项目方资料/NEXON_经济模型_Tokenomics.pdf`; its machine-readable registry is
   `../../tokenomics_assets/tokenomics.authority.json`. The project-party narrative addendum is
   `../../../raw/NEXON项目方资料/NEXON_项目叙事补充_2026-09-08.md`; its registry is
   `../../narrative_assets/nexon.narrative.authority.json`. Narrative positioning may not change
   any formula, price, ratio, release, reward, redemption or burn rule. Run both parent-workspace
   validators before publishing.

## GitBook plan notes (verified 2026-09-04)

| Feature | Free | Needed? |
| --- | --- | --- |
| Git Sync | ✅ included | required |
| **Site variants** (multiple spaces on one site, for localization) | ✅ included | **this is how EN/ZH is published** |
| Site sections | ❌ Ultimate, $249/site/mo | avoid — do not wrap the spaces in a `type: section` |
| Custom domain (e.g. `docs.nexon.markets`) | ❌ Premium, $65/site/mo | needed before public launch |
| PDF export | ❌ Premium | not needed — we render the PDF from this repo ourselves |
| Redirect management (UI) | ❌ Premium | `.gitbook.yaml` redirects are git-driven, unaffected |

GitBook rewrites `gitbook-docs.yaml` whenever the content mapping is saved in its UI.
If it does, `git pull` before editing further.
