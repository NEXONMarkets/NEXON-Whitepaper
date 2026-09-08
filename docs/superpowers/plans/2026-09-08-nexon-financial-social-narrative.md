# NEXON Financial-Social Narrative Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Expand NEXON’s bilingual whitepaper and knowledge system around the approved “new-generation value connection network” thesis, keeping project-approved economics primary, AI-native PayFi secondary, and all five ecosystem products explicitly Roadmap.

**Architecture:** Maintain two linked authorities: a narrative registry for brand meaning, asset positioning and product direction, and the existing tokenomics registry for formulas and executable economics. Public copy follows a concentric story—three disconnected markets, dual assets, approved mechanics, AI-native PayFi, then the financial-social product ecosystem—while validators prevent roadmap claims from becoming current capabilities.

**Tech Stack:** Markdown/GitBook, JSON authority registries, Python 3 `unittest` validators, existing whitepaper lint/compliance scripts, Git.

**Spec:** `docs/superpowers/specs/2026-09-08-nexon-financial-social-narrative-design.md`

## Global Constraints

- Economic mechanics remain controlled by `raw/NEXON项目方资料/NEXON_经济模型_Tokenomics.pdf`, dated 2026-09-06, SHA-256 `4a6de040273eeb2a9b921654ae289d36fa0377adf5d5c48a93ce431d5ed65d6a`.
- Narrative positioning follows the project-party written addendum supplied on 2026-09-08: “NEXON 是生态，XO 承载价值，EXON 驱动流通。”
- XO is the narrative value anchor and the current staking-principal carrier; governance and broader rights remain Roadmap/Open until rules are published.
- EXON is the narrative circulation engine and the current spot/release/buy/check/burn asset; payment, exchange, fee and consumption utility remain Roadmap until product terms are published.
- AI-Native PayFi is the secondary narrative focus. Wallet, Marketplace, Stablecoin Card and decentralized Social App are ecosystem extensions.
- PayFi, Wallet, Marketplace, Stablecoin Card and Social App all default to `Roadmap`; none may be called live or launched without new evidence.
- Do not invent EXON total supply, complete allocation, initial float, future-round quotas, governance thresholds, card issuer, product dates or dynamic-reward level tables.
- Keep every APY, price, ROI, payback and yield illustration adjacent to conditions and principal-loss risk.
- Preserve raw source files and historical archives unchanged.

---

### Task 1: Establish a failing narrative documentation contract

**Files:**
- Create: `/Users/ericc/Desktop/土豆/Vita/tests/test_narrative_docs.py`
- Test: `/Users/ericc/Desktop/土豆/Vita/tests/test_narrative_docs.py`

**Interfaces:**
- Consumes: project root and a future validator at `output/narrative_assets/validate_docs.py`.
- Produces: one repository-level contract test whose stdout must contain `NEXON NARRATIVE CHECK PASSED`.

- [ ] **Step 1: Write the failing test**

```python
import subprocess
import sys
import unittest
from pathlib import Path

ROOT = Path(__file__).resolve().parents[1]
VALIDATOR = ROOT / "output/narrative_assets/validate_docs.py"


class NarrativeDocumentationContractTest(unittest.TestCase):
    def test_narrative_authority_and_public_docs_are_aligned(self):
        result = subprocess.run(
            [sys.executable, str(VALIDATOR)],
            cwd=ROOT,
            text=True,
            capture_output=True,
        )
        self.assertEqual(result.returncode, 0, result.stderr or result.stdout)
        self.assertIn("NEXON NARRATIVE CHECK PASSED", result.stdout)


if __name__ == "__main__":
    unittest.main()
```

- [ ] **Step 2: Run the test and confirm the red state**

Run: `python3 -m unittest tests/test_narrative_docs.py -v`

Expected: failure because `output/narrative_assets/validate_docs.py` does not exist.

### Task 2: Archive the narrative addendum and create its machine authority

**Files:**
- Create: `/Users/ericc/Desktop/土豆/Vita/raw/NEXON项目方资料/NEXON_项目叙事补充_2026-09-08.md`
- Create: `/Users/ericc/Desktop/土豆/Vita/output/narrative_assets/nexon.narrative.authority.json`
- Create: `/Users/ericc/Desktop/土豆/Vita/output/narrative_assets/validate_docs.py`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/tokenomics_assets/tokenomics.authority.json`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/tokenomics_assets/CONFLICT_AUDIT.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/raw/NEXON项目方资料/README.md`
- Test: `/Users/ericc/Desktop/土豆/Vita/tests/test_narrative_docs.py`

**Interfaces:**
- Consumes: exact project-party copy supplied on 2026-09-08 and the existing tokenomics registry.
- Produces: a narrative JSON registry with keys `source`, `brand`, `assets`, `product_thesis`, `product_status`, `boundaries`, and `economic_authority`.

- [ ] **Step 1: Save the supplied project-party narrative as an immutable source note**

Record the NEXON, XO and EXON name meanings, three-market narrative, dual-asset narrative, English tagline and the exact line `NEXON 是生态，XO 承载价值，EXON 驱动流通。` Add provenance stating that this was supplied as project-party-approved written information on 2026-09-08; do not blend analysis into the source block.

- [ ] **Step 2: Create the narrative authority registry**

The JSON must encode these exact status decisions:

```json
{
  "product_status": {
    "ai_native_payfi": "roadmap_secondary_focus",
    "wallet": "roadmap",
    "marketplace": "roadmap",
    "stablecoin_card": "roadmap",
    "decentralized_social": "roadmap"
  },
  "economic_authority": {
    "registry": "output/tokenomics_assets/tokenomics.authority.json",
    "rule": "Narrative positioning may not change formulas, prices, ratios, release, reward, redemption or burn mechanics."
  }
}
```

The asset records must separately store `narrative_role`, `current_mechanical_role`, and `roadmap_utility`.

- [ ] **Step 3: Link the tokenomics registry back to the narrative registry**

Add a top-level `narrative_context` object containing the narrative registry path and a statement that the 2026-09-08 addendum controls brand semantics while the PDF controls economic execution.

Update `CONFLICT_AUDIT.md` with the two-authority hierarchy and the rule that the new narrative positioning does not change PDF arithmetic.

- [ ] **Step 4: Implement the narrative validator**

The validator must:

- verify the source note and registry exist;
- verify the five products remain Roadmap in the registry;
- require the core Chinese and English narrative markers in Wiki, EN/ZH whitepaper, project instructions and both external memories;
- reject public assertions that any of the five products is live or launched;
- reject current-tense claims that XO already grants voting rights;
- reject claims that EXON is already the universal payment or fee token;
- call `output/tokenomics_assets/validate_docs.py` and fail if the economic contract fails.

- [ ] **Step 5: Run the contract test and keep it red for missing public markers**

Run: `python3 -m unittest tests/test_narrative_docs.py -v`

Expected: failure listing the Wiki, whitepaper and memory markers not yet present.

### Task 3: Deepen the Wiki around the approved narrative

**Files:**
- Create: `/Users/ericc/Desktop/土豆/Vita/wiki/12-超级金融社交综合体叙事.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/wiki/README.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/wiki/01-实体关系.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/wiki/03-业务与生态.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/wiki/04-代币与发行.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/wiki/07-对外口径与风险隔离.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/wiki/09-资料索引.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/wiki/11-Tokenomics权威机制与收益.md`
- Test: `/Users/ericc/Desktop/土豆/Vita/tests/test_narrative_docs.py`

**Interfaces:**
- Consumes: the two authority registries.
- Produces: one canonical human-readable narrative page and cross-links from the existing mechanism pages.

- [ ] **Step 1: Write the canonical narrative page**

Use this section order: name meaning; three disconnected markets; NEXON thesis; XO value anchor; EXON circulation engine; narrative/mechanism mapping; PayFi as secondary focus; five-product Roadmap; user value loop; staged expansion; public-language boundaries.

- [ ] **Step 2: Update existing Wiki pages surgically**

Keep all approved formulas unchanged. Add explicit language that XO’s governance and EXON’s payment/fee/consumption roles are Roadmap utilities, while the PDF-defined current mechanics remain authoritative.

- [ ] **Step 3: Add registry and source links to the source index**

The source index must distinguish the 2026-09-08 narrative authority from the 2026-09-06 economic authority and state which questions each source answers.

- [ ] **Step 4: Run the narrative and tokenomics tests**

Run:

```bash
python3 -m unittest tests/test_narrative_docs.py -v
python3 -m unittest tests/test_tokenomics_docs.py -v
```

Expected: narrative test still red only for whitepaper/memory markers; tokenomics test passes.

### Task 4: Expand the English problem and connection thesis

**Files:**
- Modify: `README.md`
- Modify: `docs/en/README.md`
- Modify: `docs/en/01-the-split/README.md`
- Modify: `docs/en/01-the-split/why-nexon.md`
- Modify: `docs/en/01-the-split/three-value-languages.md`
- Modify: `docs/en/01-the-split/why-bridges-failed.md`
- Modify: `docs/en/02-the-translator/README.md`
- Modify: `docs/en/02-the-translator/intent-over-operation.md`
- Modify: `docs/en/02-the-translator/not-ai-plus-payments.md`
- Modify: `docs/en/SUMMARY.md`

**Interfaces:**
- Consumes: narrative authority and approved source wording.
- Produces: Parts I–II with NEXON name logic, three-market problem, value-connection thesis and AI-native PayFi wedge.

- [ ] **Step 1: Rebuild the English front door**

Lead with `NEXON = NEX (Nexus) + ON`, “a new-generation value connection network,” and `From Capital to Token. From Digital to Real.` Keep the independent-community-project disclaimer visible.

- [ ] **Step 2: Deepen the three-market problem**

Explain what capital markets, digital assets and real consumption each do well; then explain fragmentation in identity, liquidity, timing, custody, regulation and final delivery. Do not claim NEXON already bridges every leg.

- [ ] **Step 3: Reframe the translator as a value-connection thesis**

Use the sequence `Intent → Route → Policy Check → User Approval → Execution → Receipt`. Position AI as a control and orchestration layer, never as a return engine.

- [ ] **Step 4: Run English GitBook and compliance checks**

Run: `python3 output/白皮书/tools/run_all.py`

Expected: zero hard errors; narrative test may remain red for later chapters and memories.

Part I and Part II together should contribute approximately 5,000–5,600 English words, with new depth concentrated in the connection thesis rather than repeated market background.

- [ ] **Step 5: Commit the English thesis expansion**

```bash
git add README.md docs/en/README.md docs/en/01-the-split docs/en/02-the-translator docs/en/SUMMARY.md
git commit -m "docs: expand NEXON value connection thesis"
```

### Task 5: Make the English product stack a coherent Roadmap ecosystem

**Files:**
- Modify: `docs/en/03-architecture/README.md`
- Modify: `docs/en/03-architecture/intent-layer.md`
- Modify: `docs/en/03-architecture/agent-runtime.md`
- Modify: `docs/en/03-architecture/settlement-and-custody.md`
- Modify: `docs/en/03-architecture/trust-and-bonding.md`
- Modify: `docs/en/04-product-stack/README.md`
- Modify: `docs/en/04-product-stack/payfi.md`
- Modify: `docs/en/04-product-stack/wallet.md`
- Modify: `docs/en/04-product-stack/marketplace.md`
- Modify: `docs/en/04-product-stack/stablecoin-card.md`
- Modify: `docs/en/04-product-stack/social.md`
- Modify: `docs/en/SUMMARY.md`

**Interfaces:**
- Consumes: the five Roadmap statuses and the current economic two-layer boundary.
- Produces: architecture/product chapters organized around one user value loop.

- [ ] **Step 1: Expand the two-layer architecture**

Separate unified identity/account services, NEX Main Exchange / CEX, Staking Platform, Roadmap application orchestration and licensed/third-party execution. Explain custody and accountability per leg.

- [ ] **Step 2: Make PayFi the longest product chapter**

Cover goal capture, route preview, policy checks, scoped authority, revocation, execution receipts and failure handling. State that product fees and settlement assets will be defined by product terms; do not call EXON a current universal fee token.

- [ ] **Step 3: Expand Wallet and prediction-market boundaries**

Describe Wallet as the financial home for assets, permissions, staking access and third-party non-custodial experiences. Prediction markets remain third-party protocols subject to jurisdiction and their own rules.

- [ ] **Step 4: Expand Marketplace, Card and Social**

Marketplace connects travel, hotels, goods and services; Card requires a responsible licensed issuer/operator; Social combines communication, communities, strategy sharing and value interactions. Mark every product capability Roadmap.

- [ ] **Step 5: Add the closed-loop journey**

Use `Discover in Social → Decide in Wallet → Route through PayFi → Use in Marketplace or Card → Return with data, relationships and activity.` Explain that this is a product vision, not a live transaction claim.

- [ ] **Step 6: Run all checks and commit**

Run: `python3 output/白皮书/tools/run_all.py`

Then:

```bash
git add docs/en/03-architecture docs/en/04-product-stack docs/en/SUMMARY.md
git commit -m "docs: define the NEXON financial-social product roadmap"
```

### Task 6: Align the English dual-asset economy, roadmap and risks

**Files:**
- Modify: `docs/en/05-tokenomics/README.md`
- Modify: `docs/en/05-tokenomics/two-assets-two-jobs.md`
- Modify: `docs/en/05-tokenomics/xo.md`
- Modify: `docs/en/05-tokenomics/exon.md`
- Modify: `docs/en/05-tokenomics/value-flows.md`
- Modify: `docs/en/06-governance/README.md`
- Modify: `docs/en/07-security-and-risk/README.md`
- Modify: `docs/en/08-compliance/README.md`
- Modify: `docs/en/09-roadmap/README.md`
- Modify: `docs/en/glossary/README.md`
- Modify: `docs/en/legal-disclaimer/README.md`
- Modify: `docs/en/open-parameters/README.md`

**Interfaces:**
- Consumes: narrative/mechanical asset mapping and all PDF formulas.
- Produces: an English economic section that can state “XO anchors value; EXON activates circulation” without changing approved arithmetic.

- [ ] **Step 1: Add narrative, mechanism and Roadmap sub-sections for each asset**

XO must not be reduced to “worthless accounting principal,” and EXON must not be called the sole source of all ecosystem value. Each asset page states what is confirmed now and what is only planned.

- [ ] **Step 2: Preserve the complete economic model**

Retain 72/28, fuel check, release schedule, Base APY, term weights, early exit, redemption burn, Matching Bonus and all three worked examples verbatim in meaning and arithmetic.

- [ ] **Step 3: Replace the roadmap with capability gates**

Use four phases: economic/account foundation; AI-Native PayFi; Wallet/Marketplace/Card; decentralized financial social network. Include no calendar promise.

- [ ] **Step 4: Expand governance and product-specific risk boundaries**

State that XO governance is a direction, not a live right. Add AI authorization, prediction market, card issuer, merchant delivery and cross-jurisdiction risks.

- [ ] **Step 5: Meet the English depth target without duplicating mechanics**

Run: `python3 output/白皮书/tools/wordcount.py`

Expand thin chapters until the English manuscript reaches 19,000–22,000 words and each edited chapter is close to its configured target. Use concrete user journeys, system boundaries, failure cases and responsibility mapping; keep the detailed worked examples inside Part V.

- [ ] **Step 6: Run all checks and commit**

Run: `python3 output/白皮书/tools/run_all.py`

Then:

```bash
git add docs/en/05-tokenomics docs/en/06-governance docs/en/07-security-and-risk docs/en/08-compliance docs/en/09-roadmap docs/en/glossary docs/en/legal-disclaimer docs/en/open-parameters
git commit -m "docs: map dual-asset narrative to approved mechanics"
```

### Task 7: Produce complete Simplified Chinese parity

**Files:**
- Modify: `docs/zh/README.md`
- Modify: `docs/zh/01-the-split/README.md`
- Modify: `docs/zh/01-the-split/why-nexon.md`
- Modify: `docs/zh/01-the-split/three-value-languages.md`
- Modify: `docs/zh/01-the-split/why-bridges-failed.md`
- Modify: `docs/zh/02-the-translator/README.md`
- Modify: `docs/zh/02-the-translator/intent-over-operation.md`
- Modify: `docs/zh/02-the-translator/not-ai-plus-payments.md`
- Modify: `docs/zh/03-architecture/README.md`
- Modify: `docs/zh/03-architecture/intent-layer.md`
- Modify: `docs/zh/03-architecture/agent-runtime.md`
- Modify: `docs/zh/03-architecture/settlement-and-custody.md`
- Modify: `docs/zh/03-architecture/trust-and-bonding.md`
- Modify: `docs/zh/03-architecture/data-and-oracles.md`
- Modify: `docs/zh/04-product-stack/README.md`
- Modify: `docs/zh/04-product-stack/payfi.md`
- Modify: `docs/zh/04-product-stack/wallet.md`
- Modify: `docs/zh/04-product-stack/marketplace.md`
- Modify: `docs/zh/04-product-stack/stablecoin-card.md`
- Modify: `docs/zh/04-product-stack/social.md`
- Modify: `docs/zh/05-tokenomics/README.md`
- Modify: `docs/zh/05-tokenomics/two-assets-two-jobs.md`
- Modify: `docs/zh/05-tokenomics/xo.md`
- Modify: `docs/zh/05-tokenomics/exon.md`
- Modify: `docs/zh/05-tokenomics/distribution.md`
- Modify: `docs/zh/05-tokenomics/staking-and-returns.md`
- Modify: `docs/zh/05-tokenomics/worked-examples.md`
- Modify: `docs/zh/05-tokenomics/value-flows.md`
- Modify: `docs/zh/06-governance/README.md`
- Modify: `docs/zh/07-security-and-risk/README.md`
- Modify: `docs/zh/08-compliance/README.md`
- Modify: `docs/zh/09-roadmap/README.md`
- Modify: `docs/zh/glossary/README.md`
- Modify: `docs/zh/legal-disclaimer/README.md`
- Modify: `docs/zh/open-parameters/README.md`
- Modify: `docs/zh/SUMMARY.md`

**Interfaces:**
- Consumes: completed English information architecture and the original Chinese approved wording.
- Produces: Chinese chapters with section-level parity, natural Chinese phrasing and identical statuses/numbers.

- [ ] **Step 1: Translate by claim, not sentence shape**

Use the exact approved Chinese phrases for NEXON, XO, EXON and the core narrative. Preserve all numerical formatting and status labels.

- [ ] **Step 2: Verify chapter and heading parity**

Run: `python3 output/白皮书/tools/term_pairs.py`

Expected: zero errors and zero missing chapter pairs.

Run `python3 output/白皮书/tools/wordcount.py` and expand the Chinese manuscript to 35,000–45,000 Chinese characters with the same claim depth as English.

- [ ] **Step 3: Run all checks and commit**

Run: `python3 output/白皮书/tools/run_all.py`

Then:

```bash
git add docs/zh
git commit -m "docs: add Chinese financial-social narrative parity"
```

### Task 8: Synchronize supporting narrative documents and memories

**Files:**
- Modify: `/Users/ericc/Desktop/土豆/Vita/AGENTS.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/CLAUDE.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/白皮书/大纲-内部.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/白皮书/写作简报.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/白皮书/源文本-叙事主文档.txt`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/白皮书/源文本-话术手册.txt`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/思维导图/NEXON-思维导图-大纲.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/思维导图/nexon-mindmap.html`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/思维导图/nexon-mindmap.png`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/叙事/NEXON-叙事主文档.html`
- Modify: `/Users/ericc/Desktop/土豆/Vita/output/叙事/NEXON-全渠道话术手册.html`
- Modify: `/Users/ericc/.claude/projects/-Users-ericc-Desktop----Vita/memory/MEMORY.md`
- Modify: `/Users/ericc/.claude/projects/-Users-ericc-Desktop----Vita/memory/nexon-project.md`
- Modify: `/Users/ericc/.claude/projects/-Users-ericc-Desktop----Vita/memory/nexon-tokenomics.md`
- Create: `/Users/ericc/.claude/projects/-Users-ericc-Desktop----Vita/memory/nexon-narrative.md`
- Modify: `/Users/ericc/.codex/memories/MEMORY.md`
- Modify: `/Users/ericc/.codex/memories/memory_summary.md`
- Modify: `/Users/ericc/.codex/memories/nexon-tokenomics.md`
- Create: `/Users/ericc/.codex/memories/nexon-narrative.md`
- Test: `/Users/ericc/Desktop/土豆/Vita/tests/test_narrative_docs.py`

**Interfaces:**
- Consumes: canonical Wiki and both registries.
- Produces: concise agent instructions and durable memories that preserve both narrative and economics.

- [ ] **Step 1: Update project instructions with the dual-authority rule**

Instructions must tell future agents which source controls brand narrative and which controls economic calculations.

- [ ] **Step 2: Rewrite supporting narrative documents from the canonical structure**

Use the same hierarchy and Roadmap labels; keep the tokenomics examples intact; remove older claims that XO is only a capacity/governance token or EXON a universal route fee.

- [ ] **Step 3: Update Claude and Codex memories**

Each memory must contain the exact Chinese core line, the English master sentence, PayFi’s secondary-priority status, five Roadmap product statuses, the dual-authority source paths and the tokenomics SHA-256.

- [ ] **Step 4: Re-render and inspect the mind map PNG**

Render `output/思维导图/nexon-mindmap.html` at 1600×1000 and inspect the PNG for clipping, legibility and correct status labels.

- [ ] **Step 5: Run both contract tests**

Run:

```bash
python3 -m unittest tests/test_narrative_docs.py -v
python3 -m unittest tests/test_tokenomics_docs.py -v
```

Expected: both pass.

### Task 9: Reader-test the complete whitepaper and close gaps

**Files:**
- Create: `/Users/ericc/Desktop/土豆/Vita/output/narrative_assets/READER_AUDIT.md`
- Modify: `/Users/ericc/Desktop/土豆/Vita/wiki/12-超级金融社交综合体叙事.md`
- Modify: `docs/en/README.md`
- Modify: `docs/en/04-product-stack/README.md`
- Modify: `docs/en/05-tokenomics/README.md`
- Modify: `docs/en/09-roadmap/README.md`
- Modify: `docs/zh/README.md`
- Modify: `docs/zh/04-product-stack/README.md`
- Modify: `docs/zh/05-tokenomics/README.md`
- Modify: `docs/zh/09-roadmap/README.md`

**Interfaces:**
- Consumes: complete Wiki, EN/ZH whitepaper, registries and memories.
- Produces: an evidence table for eight reader questions plus ambiguity and contradiction results.

- [ ] **Step 1: Answer the eight acceptance questions using only maintained documents**

Record the source file and direct answer for each question listed in section 8.1 of the design spec. Mark a question failed if the answer requires hidden conversation context.

- [ ] **Step 2: Run three adversarial ambiguity checks**

Check whether a fresh reader could conclude that: the five products are live; XO governance is already active; or EXON is already mandatory for every payment. Fix copy until all three conclusions are impossible.

- [ ] **Step 3: Check for generic or duplicated filler**

Review each expanded chapter for repeated slogans, unsupported market claims and repeated tokenomics explanations. Meet the configured depth targets with concrete explanation rather than duplicated copy.

- [ ] **Step 4: Run the final repository suite**

Run:

```bash
python3 -m unittest tests/test_narrative_docs.py tests/test_tokenomics_docs.py -v
python3 output/白皮书/tools/run_all.py
git -C output/白皮书/NEXON-Whitepaper diff --check
```

Expected: all tests and hard checks pass; configured manuscript totals are met and any remaining warning is individually reviewed.

### Task 10: Commit and push the completed whitepaper branch

**Files:**
- Modify: `docs/superpowers/plans/2026-09-08-nexon-financial-social-narrative.md`
- Modify: `README.md`
- Modify: `docs/en/SUMMARY.md`
- Modify: `docs/zh/SUMMARY.md`
- Verify: the nested whitepaper repository status and remote branch.

**Interfaces:**
- Consumes: green final suite and completed reader audit.
- Produces: clean local `wp/v1-draft` matching `origin/wp/v1-draft`.

- [ ] **Step 1: Review the final diff and working tree**

Run:

```bash
git -C output/白皮书/NEXON-Whitepaper status --short
git -C output/白皮书/NEXON-Whitepaper diff --stat
git -C output/白皮书/NEXON-Whitepaper diff --check
```

Expected: only intended narrative/whitepaper changes and no whitespace errors.

- [ ] **Step 2: Commit remaining whitepaper changes**

```bash
git -C output/白皮书/NEXON-Whitepaper add README.md docs
git -C output/白皮书/NEXON-Whitepaper commit -m "docs: expand NEXON financial-social ecosystem narrative"
```

- [ ] **Step 3: Push the approved branch**

Run: `git -C output/白皮书/NEXON-Whitepaper push origin wp/v1-draft`

- [ ] **Step 4: Verify local and remote references match**

Run:

```bash
git -C output/白皮书/NEXON-Whitepaper status --short
git -C output/白皮书/NEXON-Whitepaper rev-parse HEAD
git -C output/白皮书/NEXON-Whitepaper rev-parse origin/wp/v1-draft
```

Expected: clean status and identical commit hashes.
