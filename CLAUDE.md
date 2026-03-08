# What We Know — Project Instructions

## What this is
A free, static website (whatweknow.co.uk) providing sourced, reviewed trans healthcare information for the UK. Built with Astro, hosted on Google Cloud via GitHub (harperautomation/whatweknow).

## Core principles
- **AI is backend only.** Users never interact with AI. They see clean, human-reviewed content.
- **Everything is sourced.** No claim without a reference. No reference without verification.
- **This is healthcare.** Accuracy is non-negotiable. Say "we don't know" before guessing.
- **Free forever.** No paywalls. No premium tier. This is a community resource.
- **Anonymous.** No personal names, emails, or identifying information on the public site. Contact goes through /contact form.
- **UK-focused.** Architecture supports multi-country later, but content is UK-first.
- **Harm reduction, not moralisation.** Present safety information for DIY topics without judgement.

## Privacy — CRITICAL
- **NEVER** reference Hormony, Catherine, focus groups, or any private research data on the public site
- **NEVER** include personal emails, names, or locations
- The project's connection to Hormony is private development context, not public information

## Source hierarchy
1. **Tier 1 — Clinical guidelines:** WPATH SOC-8, Endocrine Society 2017, NHS England, NICE, BNF
2. **Tier 2 — Curated community:** transfemscience.org, genderkit.org.uk, transactual.org.uk, transhub.org.au, transgendermap.com, diyhrt.wiki, transharmreduction.org
3. **Tier 3 — Community discussion:** Reddit (r/asktransgender, r/MtF, r/ftm, r/TransDIY, r/transgenderUK), Susan's Place, forums
4. **Tier 4 — Social/anecdotal:** TikTok, YouTube — trend detection only, not factual sourcing

Medical claims require Tier 1 sources. Community experience adds context but is not evidence.

## Content confidence levels
- 🟢 **Strong consensus** — Multiple Tier 1 sources agree, community aligns
- 🟡 **Emerging** — Some evidence, growing support, gaps remain
- 🟠 **Contested** — Sources disagree or clinical vs community views diverge
- 🔴 **Insufficient data** — Limited evidence, mostly anecdotal

## Topic page structure
Every topic page follows this format:
1. The short version (2-3 paragraphs)
2. What the guidelines say (Tier 1, cited)
3. What the community says (Tier 2-3, aggregated themes)
4. Where people disagree (both sides, sourced)
5. Sources (numbered, with URLs and tier labels)

## Slash commands
- `/research <question or topic>` — Launch the multi-agent research pipeline. Searches all source tiers in parallel, synthesises with confidence ratings, fact-checks every claim.

## Tech stack
- Astro (static site generator)
- Bun (package manager / runtime)
- Deployed to Google Cloud Run via Docker (nginx serving static files)
- GitHub: harperautomation/whatweknow

## Editorial process
- Charlie is the sole reviewer
- No clinical advisor yet — avoid topics requiring clinical judgement
- Prioritise topics with strong consensus from strong sources
- All content must be fact-checked against live sources before publishing

## Current topics (live)
1. NHS gender clinic waiting times
2. Changing your name (England & Wales)
3. Blood work basics

## Planned topics
4. UK private providers compared
5. What to expect from estrogen (first year)
6. What to expect from testosterone (first year)
7. Voice training: where to start
8. Hair removal: laser vs electrolysis
9. GRC application process
10. Where to find support (UK)
