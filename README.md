# KYC — Know Your Citizen

**A living, citizen-drafted document of reforms for India's education system.**

KYC hosts an open, version-controlled draft of proposed reforms, beginning with **examination integrity (NEET)** and
expanding to other areas over time.

**This is a citizen initiative. It is not affiliated with any government body,
political party, or official consultation process.**

## How it works

1. **The Draft** lives in [`/draft`](./draft). It is the consolidated,
   versioned document — the output of this whole process.
2. **Proposals** are made in
   [GitHub Discussions → Proposals](../../discussions/categories/proposals)
   using the required template (problem → evidence → proposed reform →
   tradeoffs).
3. **Voting** happens with 👍 / 👎 reactions on proposal discussions. A
   scheduled GitHub Action tallies reactions into
   [`data/proposals.json`](./data/proposals.json), which powers the public
   site. All votes are public and auditable.
4. **Merging** is done by maintainers on a monthly cadence, following the
   published criteria in [GOVERNANCE.md](./GOVERNANCE.md). Vote counts inform
   merges; they do not automate them. Every merge is recorded in
   [CHANGELOG.md](./CHANGELOG.md) with reasoning.

## Participate

- 📖 Read the current draft: start with
  [`draft/00-preamble.md`](./draft/00-preamble.md)
- 🗳️ Vote on open proposals:
  [Discussions → Proposals](../../discussions/categories/proposals)
- ✍️ Submit a proposal: read [CONTRIBUTING.md](./CONTRIBUTING.md) first
- 🔧 Fix errors or improve sourcing in the draft: open a pull request

## Principles

- **Evidence over volume.** Proposals need sources; objections need substance.
- **Transparency.** Every vote, every merge, every rule change is public.
- **Constructive by design.** We draft what should exist, not only what is
  broken.

## License

Draft content: CC BY 4.0. Code (site, workflows): MIT.
