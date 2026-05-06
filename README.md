# HigherOrder Documentation

Public product documentation for the HigherOrder platform, hosted on Mintlify.

Live site: https://higher-order.ai (production URL TBD)

## Repository structure

- `docs.json` — Mintlify configuration (theme, navigation, branding)
- `index.mdx` — landing page
- `ai-assistant.mdx` — AI Assistant
- `vendor-risk/` — Vendor Risk (inventory, contract standards, questionnaire templates)
- `customer-risk/` — Customer Risk (golden standards)
- `contract-intel/` — Contract Intel (command center, portfolio, golden standards, analytics)
- `vendor-risk-intel/` — Vendor Risk Intel (command center, portfolio, analytics)
- `contracts/` — Contracts (customer, vendor)
- `vendor-intake.mdx` — Vendor Intake
- `administration.mdx` — Administration
- `changelog/` — release notes
- `logo/`, `images/` — assets
- `CLAUDE.md` — style guide for Claude Code-assisted authoring

## Local development

```bash
npm i -g mint
mint dev
```

Deploys to Mintlify automatically on push to `main`.
