# Hi, I'm Teodor 👋

📍 **Bucharest, EU time** | 🤖 **Building agent systems that run a real business** | 🎯 **Open to remote AI Engineer roles**

Founder of [Ministeru' Creativ](https://ministerucreativ.com), a four-person agency whose back office is an agent fleet I built and operate. BSc Computer Games Design and Development (Worcester, 2022).

![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Swift](https://img.shields.io/badge/-Swift-FA7343?style=flat-square&logo=swift&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Playwright](https://img.shields.io/badge/-Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Azure OpenAI](https://img.shields.io/badge/-Azure_OpenAI-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Vercel](https://img.shields.io/badge/-Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Claude Code](https://img.shields.io/badge/-Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white)

## Start here

- 🧭 **[icp-agent](https://github.com/tiXor-code/icp-agent)** - agentic lead engagement: enrich a company, assess-loop until confident, ICP score, route, draft the email, log to a Sheet. ReAct with closed-enum actions, every failure mode handled explicitly. [Live demo](https://icp-agent-ten.vercel.app)
- 🎫 **[instantly-support-agent](https://github.com/tiXor-code/instantly-support-agent)** - support-ticket responder: RAG over an indexed help centre, self-graded drafts, a multi-signal confidence gate that decides auto-send vs human review, and the full decision chain on one page per ticket. [Live demo](https://instantly-support-agent.vercel.app) (sign-in)
- 📄 **[cv-tailor](https://github.com/tiXor-code/cv-tailor)** - job description in, tailored CV out: one structured LLM call, a deterministic Jinja/WeasyPrint renderer, an honesty guard that refuses invented experience, browser-faithful host allow-listing before any portal submit, leak-canary tests. 539 tests.
- 🚿 **[faraapacalda.ro](https://faraapacalda.ro)** - how many days a year Bucharest goes without hot water. A 15-minute git-scraper ([termo-data](https://github.com/tiXor-code/termo-data)) feeds a 2,350-page static site ([termo-site](https://github.com/tiXor-code/termo-site)) with real users and a feedback loop.
- 🎧 **[ColdCoach](https://github.com/tiXor-code/coldcoach)** - live coaching for cold calls, native macOS: on-device WhisperKit transcription, coaching cards within ~2 s of an objection, a playbook that learns from logged outcomes, bring your own key. Homebrew tap, CalVer releases.
- 🧠 **[wiki-substrate](https://github.com/tiXor-code/wiki-substrate)** - the memory substrate my agents run on: a typed markdown schema, ingest and lint tooling, and MCP wiring over Tobi Lutke's [qmd](https://github.com/tobi/qmd).

## Projects

### Agents and LLM systems

- 🧭 **[icp-agent](https://github.com/tiXor-code/icp-agent)** - enrich, assess, score, route, email, log; an agent that knows when it has enough
- 🎫 **[instantly-support-agent](https://github.com/tiXor-code/instantly-support-agent)** - RAG plus a confidence gate that knows when to hand off to a human
- 📄 **[cv-tailor](https://github.com/tiXor-code/cv-tailor)** - structured output, deterministic rendering, an honesty guard
- 🧠 **[wiki-substrate](https://github.com/tiXor-code/wiki-substrate)** - schema and MCP wiring for a markdown vault used as agent memory

### Data pipelines and civic tech

- 🗄️ **[termo-data](https://github.com/tiXor-code/termo-data)** - git-scraper: CMTEB outage pages snapshotted every 15 minutes since June 2026, committed only on change
- 🚿 **[termo-site](https://github.com/tiXor-code/termo-site)** - pure-SSG Next.js site over that archive, street and heating-point level, 122 tests plus Playwright e2e

### Native and tools

- 🎧 **[ColdCoach](https://github.com/tiXor-code/coldcoach)** - Swift, WhisperKit, floating overlay, Keychain-stored keys
- 🍺 **[homebrew-coldcoach](https://github.com/tiXor-code/homebrew-coldcoach)** - `brew install --cask tiXor-code/coldcoach/coldcoach`

### Web apps

- 🚀 **[eve-arbitrage](https://github.com/tiXor-code/eve-arbitrage)** - inter-region hauling arbitrage in EVE Online, ranked by exact profit per trip after walking the real ESI order books. [Live](https://eve-arbitrage-six.vercel.app)
- 📐 **[room-planner](https://github.com/tiXor-code/room-planner)** - drag-and-drop room planner on react-konva: rooms, furniture, doors, snapping, undo/redo, JSON import/export. [Live](https://room-planner-puce.vercel.app)

### University era

- 🏚️ **[Puzzle-Haunt](https://github.com/tiXor-code/Puzzle-Haunt)** - final-year thriller puzzle game set in the Worcester Royal Infirmary, on a hand-rolled MonoGame engine (C#)
- 🏰 **[The-City](https://github.com/tiXor-code/The-City)** - tower defence in Unity, built for fun

## Private systems

Most of what I build runs my own company and stays private:

- **AIOS** - the agent fleet behind Ministeru' Creativ: a health sentinel with heartbeats, a 298-rule secure development reference enforced by four scanners that file findings as issues, an invoice auto-filer, a Telegram job spine running headless Claude workers, and a phone-first decision cockpit. ~970 tests.
- **Trading research** - automated micro-futures and prediction-market strategies with a settlement-truth ledger and a fail-closed risk layer.
- **Client work** - sites, booking systems and lead pipelines for agency clients, through [Ministeru' Creativ](https://ministerucreativ.com).

## How I build

- Spec, then plan, then review-gated implementation by subagents. Every build is test-gated and the test count is part of the report.
- Headless agents on launchd with heartbeats, a health sentinel and quiet hours. Nothing runs armed without a kill switch.
- A security gate on every change: a written rules reference is checked before a task is called done, and every finding carries an ID and a severity.
- A 700-page markdown wiki is the operating memory for every session. The agents read it before they act.

## Connect

[![Website](https://img.shields.io/badge/-teodorlutoiu.com-FF5722?style=flat-square&logo=googlechrome&logoColor=white)](https://teodorlutoiu.com)
[![LinkedIn](https://img.shields.io/badge/-Teodor_Lutoiu-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/teodorlc)
[![Email](https://img.shields.io/badge/-contact@teodorlutoiu.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:contact@teodorlutoiu.com)
[![GitHub](https://img.shields.io/badge/-Follow-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/tiXor-code)
