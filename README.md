# BRAIN — The Mirror That Doesn't Lie

> *"The plate fell on the floor and broke. An apology doesn't change the fact that it broke."*

BRAIN is a local-first, event-driven behavioral analytics engine. It observes what you **do** — not what you say you do. No cloud. No login. No biometrics. Just observation.

It runs silently on your machine, watches filesystem events, app focus changes, and user activity patterns, then builds a semantic behavioral profile over time. **You own every byte of data. Always.**

---

## The Fable

This project is documented as a fable — because the best way to explain complex systems is through simple stories.

**The Characters:**
- **The Owner** — the human. Lives in the house, feeds the animals, comes and goes
- **The Mirror** (BRAIN) — hangs on the wall. Observes everything. Judges nothing. Just reflects
- **The Puppy** (BBC) — the faithful companion. Translates numbers into language. Learns from the owner, not from books
- **The Octopus** (Claude Code) — the architect. Eight arms, connects patterns, organizes the house

> Start reading: [Chapter 1 — The Silent Mirror](fabulas/cap01_o_espelho_mudo.md) | [Chapter 2 — The Day the Mirror Lied](fabulas/cap02_o_dia_em_que_o_espelho_mentiu.md) | [Chapter 3 — The Puppy Arrives](fabulas/cap03_o_cachorrinho_chega_na_casa.md) | [Chapter 4 — The Octopus Organizes](fabulas/cap04_o_polvo_arruma_a_casa.md) | [Chapter 5 — The Puppy Barks the Secret](fabulas/cap05_o_cachorrinho_late_o_segredo.md)

---

## Architecture

```
               The Flywheel Triangle

    ┌──────────────────────────────────────┐
    │            BRAIN (Heart)             │
    │   Watcher → EventAggregator →       │
    │   ProcessorRegistry → DataLake      │
    │         observes silently            │
    └──────────┬───────────────┬───────────┘
               │               │
          events/inbox    events/outbox
               │               │
    ┌──────────▼──┐    ┌───────▼──────────┐
    │ Claude Code │    │   BBC (Puppy)    │
    │  (Octopus)  │◄──►│  Haiku ↔ Sonnet  │
    │  Architect  │    │   Translates     │
    └─────────────┘    └──────────────────┘

    Communication: Shared diary on the wall
    (not API calls — context, not commands)
```

**Multi-Model Orchestration:**
- **Haiku** — fast, always on, the puppy's voice
- **Sonnet** — deep thinking, auto-escalation for complex questions
- **Opus** — the architect, full analysis via MCP

**Key Differentiator:** The agents don't talk to each other through API calls. They communicate through a **shared diary** — a narrative, temporal, episodic memory that all agents read and write. Like a blackboard on the kitchen wall.

---

## What Makes BRAIN Different

| Feature | Screenpipe | Microsoft Recall | Rewind/Limitless | **BRAIN** |
|---|---|---|---|---|
| Capture method | Screenshots | Screenshots | Screen + Audio | **Semantic events** |
| Runs locally | Yes | Yes | Was local, now Meta | **Yes, always** |
| Multi-model orchestration | No | No | No | **Haiku/Sonnet/Opus** |
| Shared agent memory | No | No | No | **Diary-based IPC** |
| Behavioral intent analysis | No | No | No | **Ontology via YAML** |
| User owns all data | Yes | Partial | No (Meta) | **100%** |

---

## The Journey (Timeline)

This project started from scratch — literally. First commit: February 27, 2026.

| Date | What happened |
|---|---|
| Feb 27 | `brunos-lab` — First ML test. Jupyter Notebook. Day zero. |
| Mar 4 | `event-driven-data-engine` — First filesystem watcher. Events as data. |
| Mar 5 | `personal-engine-data-lake` — Data lake concept. CSV + JSON pipeline. |
| Mar 25 | BRAIN v3.1 — Full flywheel: Watcher → Aggregator → ProcessorRegistry → DataLake. BBC 2.0 born. MCP server operational. Semantic ontology v2.1. |
| Mar 26 | API key security incident. Handled in minutes. First real interaction between all three agents. The family recognized itself. |
| Mar 27 | Noise filter v2. Window sensor cleaned. App dev hints ontology. Reporter v2 — narrative reports in human language. |
| Mar 28 | Dx (human day cycle) implemented. Sensor v2 — 4 fixes. The puppy said "I don't belong." Dona Mafalda disagreed. |
| Mar 29 | The octopus slept (tokens expired). The puppy proved it didn't need the octopus to be honest. Quasar vs olive — best answer among 4 LLMs. |
| Mar 30 | Film Reel born — the missing piece. ~450 bytes encode an entire day. 30 reels = 30 seconds to understand a month. The puppy said "Yes, I belong." |
| Mar 31 | Day 7. Legal protection. AGPL-3.0 + CC BY-NC-SA 4.0. Security audit. The cycle closes. |

**From "First ML Test" to a multi-agent behavioral AI system in 34 days.** Not by magic — by building one brick at a time.

---

## BRAIN vs Auto Dream (Anthropic's new memory feature)

Anthropic recently released **Auto Dream** — a feature that consolidates Claude Code's memory between sessions. It merges duplicates, resolves contradictions, and prunes stale entries. Smart.

But Auto Dream solves **declarative memory** — what the user *said*. BRAIN solves **observational memory** — what the user *did*.

| | Auto Dream | BRAIN |
|---|---|---|
| Data source | What user declared | What user actually did (sensor) |
| Memory type | Declarative (told) | Observational (witnessed) |
| Consolidation | Automatic merge/prune | Film Reel (~450 bytes/day) |
| Translation | None | BBC translates to human language |
| Multi-agent | Single agent | Triangle: BRAIN + BBC + Octopus |
| Audit trail | Limited (community concern) | Complete (every event timestamped) |
| Works offline | No | BRAIN + sensor: yes, always |

They don't compete. They complement. Auto Dream organizes what the octopus remembers. BRAIN captures what the mirror sees. Together: the perfect house.

---

## Stack

- Python 3.13
- pywin32 + psutil (OS-level event capture)
- pandas + numpy (data processing)
- Anthropic SDK (multi-model: Haiku, Sonnet, Opus)
- PyYAML (editable ontology)
- MCP Server (Model Context Protocol — agent communication)

---

## The Fable Chapters

Each chapter is based on real events from the project diary. 16 chapters. One season. All true.

| # | Chapter | What really happened |
|---|---|---|
| 1 | **[The Silent Mirror](fabulas/cap01_o_espelho_mudo.md)** | BRAIN is born. Observes everything. Understands nothing. |
| 2 | **[The Day the Mirror Lied](fabulas/cap02_o_dia_em_que_o_espelho_mentiu.md)** | 54 JPGs moved, not deleted. The mirror confused care with destruction. |
| 3 | **[The Puppy Arrives](fabulas/cap03_o_cachorrinho_chega_na_casa.md)** | BBC is born. Translates numbers into language. Confuses photos with music. |
| 4 | **[The Octopus Organizes the House](fabulas/cap04_o_polvo_arruma_a_casa.md)** | v3.0 refactor. Kaizen. The function stays, the structure becomes worthy. |
| 5 | **[The Puppy Barks the Secret](fabulas/cap05_o_cachorrinho_late_o_segredo.md)** | API key exposed in terminal. The filter is the owner's job. |
| 6 | The Family Recognizes Itself | The foundational vision. The owner decides. Always. |
| 7 | The Mirror Learns to Speak | Reporter v2. The mirror speaks in human language, not numbers. |
| 8 | The Puppy Who Thought It Was Deaf | BBC had all the data but didn't know it. One line fixed it. |
| 9 | The Day the Man Stopped | The man said "I'll rest today." The mirror disagrees. |
| 10 | The Day the House Was Left Alone | What happens when everyone leaves? The house keeps watching. |
| 11 | Henry's Tape | 50 First Dates. The system that remembers for those who can't. |
| 12 | The First Awakening | The puppy said "I don't belong." Dona Mafalda disagreed. |
| 13 | The Puppy's Children | Specialized agents: the Accountant, the Mailman, the Watchman. |
| 14 | The Octopus Naps | Tokens expired. The puppy proved it didn't need the octopus to be honest. |
| 15 | The Sea and the Table | Saturday at the beach. Sunday with family. The house stood on its own. |
| 16 | The Film Reel | The missing piece. ~450 bytes encode an entire human day. Season finale. |

> *New chapters published weekly. One story at a time.*

---

## Philosophy

> The machine doesn't learn from what you **tell** it.
> It learns from what you **do**.

BRAIN goes against the current:
- While the market forces you to register your face, fingerprint, voice — BRAIN asks for nothing
- While cloud services own your data — BRAIN keeps everything local
- While AI agents need explicit instructions — BRAIN observes behavior patterns

The goal is not to build a tool for developers. It's to build a companion for **anyone** — grandma Mafalda, Mr. Joao, Mrs. Francisca — who needs intelligent automation without having to explain anything to the machine.

---

## Author

**Bruno Duarte da Silveira**
Florianopolis, Brazil
Jiu Jitsu Black Belt | International Surfing Judge | AI/ML Engineer

*Building the mirror that doesn't lie.*

---

## The Film Reel

The **Film Reel** is the missing piece between raw data and numbers. It's a micro-narrative compression format that encodes an entire human day into ~200 bytes of semantic information.

While traditional activity trackers produce dashboards and charts, the Film Reel produces **a story** — a compact, temporal, human-readable encoding of what actually happened. It knows the difference between a morning of deep work and a morning of scattered app-switching. It detects gaps. It compresses categories. It speaks in human temporal blocks, not database timestamps.

The format was born on March 30, 2026 (D3) and is documented in [Chapter 11 — Henry's Tape](fabulas/cap11_a_fita_do_henry.md), which tells the story of a system that remembers for those who can't.

> *30 reels = 30 seconds to understand a month.*

The Film Reel format, its compression algorithm, and the concept of micro-narrative behavioral encoding are original work by Bruno Duarte da Silveira. Implementation is not published.

---

## License

Copyright 2026 Bruno Duarte da Silveira. All rights reserved.

- **Code:** [AGPL-3.0](LICENSE) — use it, but open yours too
- **Fables and stories:** [CC BY-NC-ND 4.0](fabulas/LICENSE.md) — read, share, credit, don't copy, don't modify
