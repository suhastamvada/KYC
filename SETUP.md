# Setup (one-time, ~30 minutes)

## 1. Create the repo
- Create a public repo named `KYC` and push these files
  to the `main` branch.

## 2. Enable Discussions and categories
- Repo → Settings → General → Features → check **Discussions**.
- Open the Discussions tab → pencil icon on categories → create a category
  named exactly **Proposals** (format: *Open-ended discussion*). Keep
  **General** and add **Meta**.
- The proposal form template is already in
  `.github/DISCUSSION_TEMPLATE/proposals.yml` and applies automatically.

## 3. Turn on the workflows
- Actions tab → enable workflows if prompted.
- Settings → Actions → General → Workflow permissions → **Read and write
  permissions** (the tally bot commits `data/proposals.json`).
- Run **Tally proposal votes** once manually (Actions → select → Run
  workflow) to verify it commits the JSON.

## 4. Configure the site
- Edit `site/index.html`: set `REPO` to `suhastamvada/KYC`.
- Settings → Pages → Source: **GitHub Actions**. The `pages.yml` workflow
  deploys the `site/` folder on every push.

## 5. Point suhastamvada.com at it
At your DNS provider:
- **Apex domain** (`suhastamvada.com`): four A records →
  185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
- **www** (optional): CNAME → `suhastamvada.github.io`
Then Settings → Pages → Custom domain: `suhastamvada.com` → save →
check **Enforce HTTPS** once the certificate is issued (can take an hour).
The `site/CNAME` file is already in place so deploys keep the domain.

> If you'd rather keep suhastamvada.com for personal use, use a subdomain
> like `reforms.suhastamvada.com` (single CNAME record → suhastamvada.github.io,
> and update `site/CNAME` to match).

## 6. Before announcing
- Set the launch date in `draft/00-preamble.md`.
- Strengthen citations in the three [Seed] sections — committee report,
  court records, credible press. This is your credibility on day one.
- Pin a welcome discussion linking CONTRIBUTING.md and GOVERNANCE.md.

## Launch checklist
- [ ] Repo public, Discussions on, **Proposals** category exists
- [ ] Tally workflow ran and committed `data/proposals.json`
- [ ] Site live on Pages, REPO constant set, domain resolving with HTTPS
- [ ] Seeds cited, launch date set, welcome post pinned
