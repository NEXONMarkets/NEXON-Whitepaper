# NEXON Whitepaper

Source of truth for the NEXON whitepaper, in English and Simplified Chinese.
Published through GitBook via Git Sync — **this file is not part of the published site.**

## Layout

```
gitbook-docs.yaml            site-level mapping (spaces, languages)
docs/en/                     English space   → .gitbook.yaml · README.md · SUMMARY.md
docs/zh/                     Chinese space   → .gitbook.yaml · README.md · SUMMARY.md
docs/{en,zh}/.gitbook/assets/  cover + data charts (one copy per space)
```

The two trees use identical file paths, so every chapter has a 1:1 counterpart.
Adding a chapter means adding it to **both** trees and to **both** `SUMMARY.md` files.

## Assets

| File | Where it appears |
| --- | --- |
| `cover.svg` | Space cover (brand key visual) |
| `chart-72-28-split.svg` | Cover page · Value Flows |
| `chart-term-weights.svg` | Staking & Reward Layer · Staking & Returns |
| `chart-term-rewards.svg` | Worked Examples |
| `chart-redemption-lanes.svg` | Staking & Reward Layer · Worked Examples |
| `chart-linear-release.svg` | Distribution & Release |
| `chart-early-round-tiers.svg` | Distribution & Release |

Charts are standalone SVG — no script, no webfont, no external request — so they render
identically in GitBook, in a PDF export and in a plain browser. Every figure in them comes
from the approved Tokenomics; changing a number means regenerating the chart in **both**
`docs/en/.gitbook/assets/` and `docs/zh/.gitbook/assets/`.

## Working rules

1. **Git Sync is bi-directional.** Edit either in the repo or in the GitBook editor — never
   both at once, or you will get conflicting commits. After the first sync, `git pull`:
   GitBook normalises Markdown and will have rewritten files.
2. **`README.md` files are managed here, not in GitBook.** Editing them in the GitBook editor
   creates duplicate pages.
3. **Assets are not shared between spaces.** An image used in both languages needs a copy in
   `docs/en/.gitbook/assets/` *and* `docs/zh/.gitbook/assets/`.
4. **Never change a `key` in `gitbook-docs.yaml`.** See the warning in that file.
5. **Chinese `##`/`###` headings carry an explicit anchor** (`<a href="#slug" id="slug">`),
   using the slug of the matching English heading. GitBook cannot generate a usable anchor
   from CJK text, so without this, cross-links into a Chinese section break.
6. **Narrative and mechanical roles are both fixed.** In the narrative, NEXON is the ecosystem,
   XO carries long-term value and EXON drives circulation. In the current mechanism, XO is the
   Staking Principal Token and EXON is the Core Value Token. Both languages must preserve this
   distinction and stay structurally aligned.
7. **Two linked sources of truth.** The economic source PDF is
   `../../../raw/NEXON项目方资料/NEXON_经济模型_Tokenomics.pdf`; its machine-readable registry is
   `../../tokenomics_assets/tokenomics.authority.json`. The narrative addendum is
   `../../../raw/NEXON项目方资料/NEXON_项目叙事补充_2026-09-08.md`; its registry is
   `../../narrative_assets/nexon.narrative.authority.json`. Narrative positioning may not change
   any formula, price, ratio, release, reward, redemption or burn rule.

## Checks

```bash
python3 ../tools/run_all.py
```

Runs the GitBook lint (liquid nesting, mermaid, card tables, Chinese anchors, SUMMARY coverage,
link targets), the term-pair and dual-asset role tests, the tokenomics and narrative authority
validators, and the length report.

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
