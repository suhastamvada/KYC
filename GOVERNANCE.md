# Governance

This document defines how proposals become part of the Draft. It is published
before launch so the rules cannot be changed mid-game without a visible commit.

## Roles

- **Maintainer** (currently: the repository owner). Applies the merge criteria,
  runs the monthly merge cycle, moderates per the Code of Conduct. As the
  project grows, 2–4 additional maintainers with relevant backgrounds
  (education, law, policy, exam administration) will be added by public
  nomination.
- **Contributors**: anyone with a GitHub account. May propose, vote, comment,
  and open pull requests against the draft.

## The merge cycle

On the **first weekend of each month**, the maintainer reviews all proposals
that meet the eligibility bar and either merges them into the draft, defers
them with a stated reason, or closes them with a stated reason. Every decision
is logged in [CHANGELOG.md](./CHANGELOG.md).

## Merge criteria

A proposal is eligible for merging when **all** of the following hold:

1. **Format**: it follows the proposal template (problem, evidence, proposed
   reform, tradeoffs, affected parties).
2. **Support**: sustained net support (👍 minus 👎) over at least **21 days**,
   not just a spike. The bar scales with participation; early on, net +10 with
   a 3:1 ratio is indicative, and the maintainer will publish the bar used in
   each cycle's changelog entry.
3. **No unaddressed factual objection**: if a comment identifies a factual
   error or a cited source that does not support the claim, the proposal is
   not merged until the author addresses it.
4. **Scope**: it concerns India's education system and proposes something
   actionable (a rule, structure, process, or resource change) — not a
   sentiment, slogan, or grievance without remedy.

Vote counts **inform** merges; they do not trigger them automatically.
Automated merging is deliberately excluded because reaction counts are cheap
to manipulate. The maintainer's discretion is bounded by this document and
made auditable through the changelog.

## Anti-manipulation measures

- Voting requires a GitHub account; all reactions are publicly attributable.
- Tallies (in `data/proposals.json`) record counts per proposal; anyone can
  independently verify them against the Discussions page.
- If a cycle shows evidence of coordinated inauthentic voting (mass
  new-account reactions, vote spikes correlated with off-platform calls to
  brigade), the maintainer may discount those votes and must say so, with
  evidence, in the changelog.
- Sustained-support windows (21 days) blunt spike-based manipulation.

## Amending the draft outside the cycle

Pull requests that fix typos, broken links, or sourcing errors may be merged
at any time. Substantive changes go through the proposal process.

## Amending this document

Governance changes are proposed in Discussions under **Meta**, held open for
comment for 30 days, and merged only with a changelog entry explaining the
rationale.
