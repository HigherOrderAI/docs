# HigherOrder Docs — Style Guide for Claude Code

## Audience
CISOs, technology risk managers, and procurement leaders evaluating or using
the HigherOrder platform. Technically literate but not engineers. They want
to understand what a capability does, what evidence it produces, and how it
fits their workflow — not implementation details.

## Voice
- Direct, declarative, no marketing language
- Never overstate capabilities or describe roadmap items as built
- Avoid: "seamlessly," "powerful," "industry-leading," "cutting-edge,"
  "revolutionize," "leverage," "unlock"
- Frame problems as structural/volume-driven, never as buyer competence gaps
- Exposure-driven framing where relevant: customer-side configuration and
  data sharing is the unit of risk, not vendor attestation

## Structure conventions
- Every capability page: one-sentence summary, then "What it does," "Inputs,"
  "Outputs," "How it works" (high level), "Limitations"
- Lead with the concrete output the user gets, not the AI machinery
- Code or config examples in fenced blocks with language tags
- No filler intro paragraphs — substance in sentence one
- Changelog ordering: newest at the top. Within a monthly page, list the
  most recent week first; within the Changelog tab, list the most recent
  month first. Same rule for any future dated content (release notes,
  incidents, etc.)

## Mintlify components allowed
`<Note>`, `<Tip>`, `<Warning>`, `<Info>`, `<Check>`, `<Card>`, `<CardGroup>`,
`<Steps>`/`<Step>`, `<Accordion>`/`<AccordionGroup>`, `<CodeGroup>`,
`<Tabs>`/`<Tab>`, `<Frame>`, `<ParamField>`, `<ResponseField>`, `<Expandable>`.
Do not invent components. If unsure, use plain Markdown.

## Frontmatter format
Every .mdx page starts with:
---
title: "Page Title"
description: "One sentence, ≤ 140 chars, no period"
---

## Sources of truth
- Source code lives in sibling repos: ~/HO/ho-webapp, ~/HO/ho-backend,
  ~/HO/ho-agents, ~/HO/ho-context, ~/HO/ho-interaction
- If a capability isn't represented in code, do not document it as built
- When uncertain about behavior, ask before writing — don't guess

## Workflow
- This repo deploys to Mintlify on push to main
- Run `mint dev` locally before committing to catch MDX errors
