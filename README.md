<div align="center">

# Hey, I'm Johnny 👋

### I build software end to end and run it in production.

Multi-tenant SaaS · real-time lead pipelines · multiplayer game servers · a C++ network simulator that follows the RFCs

[![Portfolio](https://img.shields.io/badge/Portfolio-johnnyr.dev-0b0b0b?style=for-the-badge&logo=googlechrome&logoColor=white)](https://johnnyr.dev)
[![FrontierPixel](https://img.shields.io/badge/Studio-FrontierPixel-1f6feb?style=for-the-badge)](https://www.frontierpixel.com)
[![Email](https://img.shields.io/badge/Email-engineer%40johnnyr.dev-d14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:engineer@johnnyr.dev)

**Since June 2026: 4,400+ commits · 1,600+ merged pull requests · 17 repositories**

</div>

---

I run [**FrontierPixel**](https://www.frontierpixel.com), a studio where I take real business problems from
first conversation to production: data model, UX, integrations, deploys, and the support after launch. I'm
self-taught (I built my first PC at 10 and haven't stopped taking things apart). I'm working toward an associate
degree now, with a CS bachelor's after that.

## 🛠️ What I'm building

### FrontierPixel CRM: multi-tenant operations platform *(private, in production)*

The CRM and client-site backend FrontierPixel runs for its clients. Every business works in its own tenant with
its own modules, branding and installable home-screen app. Leads, quotes, SMS, email, calls, follow-ups, consent
records and audit history all live in one workspace.

- **Autopilot**: AI-drafted SMS and email replies, supervised in the composer, with guards on what can be offered
  and a check with staff before booking a handoff.
- **Delivery pipeline**: an isolated Convex backend for every preview branch, a schema-compatibility gate before
  every deploy, and dependency audits in CI. Merging to `main` is a production deploy.
- **Reliability work**: SMS retry and timeout handling, push alerts filtered by sender, crash-proof settings
  across stale tabs, and A2P 10DLC SMS consent.
- **208 merged PRs**

`Next.js 16` `React 19` `TypeScript` `Convex` `Better Auth` `Twilio` `Zoho` `Web Push` `Sentry`

### [Shed 210](https://www.shed210.com): production quote and lead system

A local-service site that sells: an in-browser 3D shed configurator, server-side pricing, structured quote
capture, live Google reviews, SEO content infrastructure, and instant handoff to the CRM.

- **$196,042 in conservative quoted pipeline** from 40 deduplicated, qualified opportunities in a measured
  two-month campaign (pipeline, not booked revenue)
- **1-second median** dealer alert time across 70 production notifications
- Security hardening (CSP, intake validation), review-request flow with tracked link opens, **517 merged PRs**

`Next.js` `TypeScript` `Three.js` `Convex` `Zod` `Twilio` `Zoho` · [Case study →](https://www.frontierpixel.com/work/shed-210)

### Multiplayer game server: a persistent online city *(private)*

A whole city's worth of game systems, built from scratch: **115 custom Lua modules** and **881 merged PRs in its
first three weeks**.

- **Economy**: a stock market driven by in-game events, supply-and-demand pricing, and businesses players buy
  and run
- **Gameplay**: missions, player careers, a controller-complete inventory rebuild, and custom in-game phone apps
- **Ops**: server-side cheat detection, an in-game bug reporter that files straight to the team's tracker, and a
  release script that backs up the database before every deploy, plus nightly backups. Every change to a
  third-party module is documented with its own on/off switch.
- **Release tooling**: a build pipeline that packages modules as standalone, dependency-checked releases

`Lua 5.4` `MariaDB` `Python` `JavaScript`

### Network Engineer Sim: a datacenter game where the network is real *(private, in development)*

A deterministic network simulator in **C++20**, with an **Unreal Engine 5.8** game on top that only draws what the
sim says is happening. You walk into a small office as the outside IT contractor, trace the cable, patch the jack,
and end the broadcast storm.

- Models Ethernet bridging (IEEE 802.1D), VLANs (802.1Q), ARP (RFC 826), DHCP (RFC 2131), ICMP, and NAT
  (RFC 3022). **Every protocol behaviour cites its RFC or IEEE section.**
- Time is integer nanoseconds, so protocol timers tick exactly. A broadcast storm runs millions of events per
  simulated second.
- Every player action is a command in an ordered log, the base for replays, co-op and automation.
- The engine-free core builds and tests in seconds. Gear specs come from real vendor datasheets.

`C++20` `Unreal Engine 5.8` `CMake` `Blender`

### [Nightdrop](https://github.com/404Dealer/nightdrop): a human approval gate for AI agents *(open source)*

**Agents propose. Humans approve. Scripts execute.** A credential-isolated layer between AI agents and the
outside world. Agents write drafts, a human approves the exact payload in Telegram, and a deterministic
executor runs only what was approved. Covers multi-account Gmail and Outlook triage, approved Trash and
unsubscribe, and an SMTP state machine that fails closed. No LLM in the execution path.

`TypeScript` `Node.js` `Zod` `grammY` `Microsoft Graph` `Linux` `systemd`

### Storybook: merged open-source contribution

[Fixed the accessibility panel's tab and highlight state across Stories ↔ Docs navigation](https://github.com/storybookjs/storybook/pull/32762),
with persistence behaviour and regression tests. Merged upstream.

<details>
<summary><b>Also shipped this year</b></summary>

- **Tech-EZ**: responsive client demo for repairs, network infrastructure and structured cabling, with visual
  regression checks
- **Homelab Pulse**: read-only Proxmox VE monitoring dashboard
- **Texas Grid Watch**: human-verified ERCOT interconnection-queue evidence and monthly reports, with isolated
  Vercel + Convex previews
- **CS2 Demo Tool**: turns Counter-Strike 2 replays into map-aware analysis bundles (events, positions, grenade
  paths, radar calibration)
- **AI evaluation tooling**: a fail-closed pipeline for designing, validating and calibrating engineering
  benchmark tasks
- **FrontierPixel.com** and **johnnyr.dev**: studio site with CRM-routed lead intake, and a Win98-themed
  portfolio with visual snapshot tests

</details>

## 🧭 How I work

- **I own the whole thing.** That runs from the schema to the deploy to the text message that didn't send at 2 a.m.
- **Fail closed.** I treat security, consent and failure states as features, not follow-ups.
- **Prove it.** Tests, CI gates, schema checks and regression checks, plus claims backed by a source: an RFC
  section, a datasheet, a measured number.
- **AI-native, with guardrails.** I run coding agents like a team. I set the architecture, write the rules and
  review every PR, and I build the tooling that keeps agents safe.
- **Leave it readable.** Small PRs, runbooks, and a written reason for every change to someone else's code.

## 🧰 Toolbox

| | |
| --- | --- |
| **Languages** | TypeScript · C++20 · Lua · Python · SQL |
| **Frontend** | React 19 · Next.js 16 · Tailwind CSS v4 · Three.js |
| **Backend & data** | Node.js · Convex · MariaDB · Zod · Better Auth |
| **Integrations** | Twilio · Zoho · Microsoft Graph · Gmail · Telegram · Stripe · Discord · Sentry |
| **Games & simulation** | Unreal Engine 5.8 · Lua game scripting · CMake · Blender |
| **Infra & quality** | Vercel · Docker · Linux / systemd · Proxmox · GitHub Actions · Playwright · Jest |

## 📡 Right now

Productizing the FrontierPixel CRM, building Network Engineer Sim's first levels, and getting the game server ready
for players.

**Open to full-stack, backend, and game/simulation engineering roles**, plus selected client work.
[Let's talk →](mailto:engineer@johnnyr.dev)
