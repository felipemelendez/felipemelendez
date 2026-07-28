<h1 align="center">Felipe Meléndez</h1>

<p align="center">
  <strong>I build entire products — from the pixel to the protocol.</strong>
</p>

<p align="center">
  Founder, FindTribe LLC &nbsp;·&nbsp; Full-stack engineer at Pilot &nbsp;·&nbsp; Milpitas, CA
</p>

<br/>

## FindTribe

Real-time navigation and coordination for large events — festivals, stadiums, marathons, F1.
Google Maps for events, with a fleet of AI agents on top and a network stack that keeps
working after the cell towers give out. Commercial product, private repo.

<p>
  <a href="https://apps.apple.com/us/app/findtribe-ai-event-navigation/id6474096912"><img src="https://img.shields.io/badge/App%20Store-Download-0D96F6?style=flat-square&logo=appstore&logoColor=white" alt="Download FindTribe on the App Store"/></a>
  <a href="https://play.google.com/store/apps/details?id=app.findtribe"><img src="https://img.shields.io/badge/Google%20Play-Download-414141?style=flat-square&logo=googleplay&logoColor=white" alt="Get FindTribe on Google Play"/></a>
  <a href="https://www.findtribe.ai"><img src="https://img.shields.io/badge/findtribe.ai-Visit-1a1a1a?style=flat-square" alt="FindTribe website"/></a>
</p>

**5.0 ★** on the App Store · free on iOS and Android

**Solo-built.** Product, design, UX, interface, both apps, the native modules and the
backend — all of it mine.

<!-- Demo / screenshots go here. -->

<br/>

### Six agents in production

| Agent | What it does |
|---|---|
| **Event assistant** | Voice and text. Answers anything about the event — where the short line is, when the headliner goes on — and teaches the app while you use it. Speech-to-speech over OpenAI's Realtime API. |
| **Itinerary agent** | Talk through your day out loud; it drafts and revises your schedule, then keeps it in sync across your whole group in real time. |
| **Map builder** | Organizers describe a venue in chat and the agent lays it out — stages, vendors, amenities, zones — without touching a map editor. |
| **Map scanner** | Photograph the paper map stapled to a fence. Computer vision reads it, calibrates it to real coordinates, and hands back a live interactive map. |
| **Game master** | Runs location-aware quests and encounters scoped to an event, with geohashed zones and a milestone pipeline. |
| **Semantic search** | Vector search over an event knowledge base, so answers cite the actual schedule instead of guessing. |

<br/>

### Built to survive no signal

A festival is a hundred thousand people sharing one saturated tower. The whole app is
designed for that.

- **Local-first data.** 55 SQLite repositories with migrations, eviction policy and
  session-bound lifecycles. Every screen reads and writes locally first — chat, itineraries,
  groups, media, lost-and-found, location history. The network is an optimization, not a
  requirement, and nothing is lost when it disappears mid-write.
- **Bluetooth LE mesh.** Messages hop phone to phone with delay-tolerant store-and-forward,
  end-to-end encrypted, deduplicated and ordered across hops, durable across app relaunch.
  Proven on device between iPhone and Android. 96 modules.
- **SOS over mesh.** An emergency broadcast that still reaches your people with no internet
  at all — admission control, carrier targeting and tombstones so it propagates once and
  stops.
- **Offline maps.** Mapbox tile packs downloaded and lifecycle-managed ahead of the gates.

<br/>

### Native depth

Six custom native modules in Swift and Kotlin — BLE mesh, BLE proximity, iOS Live Activities,
offline map switching, diagnostics — because the platform APIs this needs have no React
Native equivalent. Live Activities put your next set, your friends and an active SOS on the
lock screen without opening the app. Background geolocation, push delivery, subscriptions and
organizer sponsorship payments run on a serverless backend with scheduled jobs, event-driven
triggers and OpenAI function calling.

Around 800 test suites and 11,000 tests cover it.

<br/>

## Open source

### [llm-orchestrator](https://github.com/felipemelendez/llm-orchestrator)

Deploy a coordinated team of AI engineers to any codebase. A Claude Code plugin with a
structured workflow, two-stage code review, autonomous BLOCKED recovery, and a research gate
that verifies external APIs against current docs before specs get written.

<p>
  <a href="https://github.com/felipemelendez/llm-orchestrator"><img src="https://img.shields.io/github/stars/felipemelendez/llm-orchestrator?style=flat-square&label=stars&color=1a1a1a" alt="llm-orchestrator stars"/></a>
  <img src="https://img.shields.io/badge/license-MIT-1a1a1a?style=flat-square" alt="MIT licensed"/>
</p>

Smaller experiments in retrieval and agent tooling:
[`xpo-lm`](https://github.com/felipemelendez/xpo-lm) ·
[`rag-finance-engine`](https://github.com/felipemelendez/rag-finance-engine) ·
[`semantic-search-embeddings`](https://github.com/felipemelendez/semantic-search-embeddings) ·
[`mcp-agent-experiments`](https://github.com/felipemelendez/mcp-agent-experiments)

<br/>

## Other work

**Pilot** — full-stack engineering on financial systems, in production, at scale.

**Earlier ventures** — Phi Entertainment, an immersive planetarium venue concept, and
PhiTribe, a creative portfolio ecosystem I designed years before Behance was acquired.

**Teaching** — tutoring adults into college and mentoring at-risk youth, recognized with
congressional commendations.

<br/>

## Stack

TypeScript · Swift · Kotlin · Python · Ruby · C
<br/>
React Native / Expo · SQLite · PostgreSQL · Mapbox · OpenAI

<br/>

## Links

**[felipemelendez.com](https://www.felipemelendez.com)** — how I got here, and what I'm curious about.

**[findtribe.ai](https://www.findtribe.ai)** — FindTribe today. The original product shipped at
**[findtribe.app](https://www.findtribe.app)** as event navigation; the `.ai` domain arrived when the
agents did. Both are live.

**[LinkedIn](https://www.linkedin.com/in/felipemelendez/)**

<br/>

---

<p align="center">
  <sub>Best ideas arrive lying in the grass, looking at the stars, wondering <em>what if…</em><br/>
  Two golden retrievers supervise.</sub>
</p>

<p align="center">
  <em>"Great events don't just happen—they're engineered."</em>
</p>
