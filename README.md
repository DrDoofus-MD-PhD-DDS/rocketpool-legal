# Rocket Pool pDAO Legal Documentation Reset

This repository is a working space for Rocket Pool pDAO legal-structure research. It is not legal or tax advice.

The current research direction is **committee-first**. The goal is not to wrap the entire pDAO or create DAO leadership. The goal is to explore whether the pDAO can create a narrow legal service layer that helps people do approved work safely.

Core framing:

> We are not creating leadership. We are creating a safe way for people to do work.

## Canonical documentation

The `docs/` folder is the canonical working documentation. It should contain all information needed to understand the current proposal, the design guardrails, and the open questions for counsel.

The `drafts/` folder is optional. Drafts are communication artifacts derived from the main docs, such as a memo, charter outline, or governance proposal outline. Drafts should not contain unique assumptions or conclusions that are missing from `docs/`.

The `research-notes/` folder preserves source material and AI discussion summaries. Those notes are useful background, but they are not the current recommendation.

## Recommended reading order

For a fast understanding:

1. [`docs/01-executive-summary.md`](docs/01-executive-summary.md)
2. [`docs/12-integrated-internal-memo.md`](docs/12-integrated-internal-memo.md)
3. [`docs/11-open-questions-for-counsel.md`](docs/11-open-questions-for-counsel.md)

For the full structured analysis:

1. [`docs/00-project-overview.md`](docs/00-project-overview.md)
2. [`docs/01-executive-summary.md`](docs/01-executive-summary.md)
3. [`docs/02-current-pdao-functions.md`](docs/02-current-pdao-functions.md)
4. [`docs/03-risk-model.md`](docs/03-risk-model.md)
5. [`docs/04-entity-options-comparison.md`](docs/04-entity-options-comparison.md)
6. [`docs/05-duna-service-layer.md`](docs/05-duna-service-layer.md)
7. [`docs/06-duna-membership-and-pseudonymity.md`](docs/06-duna-membership-and-pseudonymity.md)
8. [`docs/07-duna-scope-guardrails-and-tokenomics-firewall.md`](docs/07-duna-scope-guardrails-and-tokenomics-firewall.md)
9. [`docs/08-third-party-funds-and-incentives.md`](docs/08-third-party-funds-and-incentives.md)
10. [`docs/09-tax-and-accounting-questions.md`](docs/09-tax-and-accounting-questions.md)
11. [`docs/10-language-guide.md`](docs/10-language-guide.md)
12. [`docs/11-open-questions-for-counsel.md`](docs/11-open-questions-for-counsel.md)
13. [`docs/12-integrated-internal-memo.md`](docs/12-integrated-internal-memo.md)

## Status labels used in these docs

- **Working assumption**: plausible based on current research, but not lawyer-verified.
- **Counsel question**: should be reviewed by legal or tax counsel before relying on it.
- **Design preference**: a practical preference for Rocket Pool culture and capacity, not a legal conclusion.
- **Guardrail**: a proposed limit to reduce legal, tax, conflict, or centralization risk.

## Existing root files

The older root-level AI-generated files are intentionally left in place for history. The new structure treats them as research notes, not final conclusions.

- `shell-summary.md` — early committee-first memo draft.
- `AI-how-RP-DUNA-work.md` — practical DUNA operating model note.
- `AI-discussion-RPL-fee-DUNA.md` — note on DUNA members, RPL staking, voter_share, and role separation.

## Maintenance rule

If a future draft contains a new factual assumption, legal conclusion, tax question, design guardrail, or practical recommendation, copy that point into the appropriate file under `docs/`. The docs are the source of truth; drafts are for reuse and presentation.
