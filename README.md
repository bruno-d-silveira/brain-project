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

> Read the full fable: [Chapter 1 — The Silent Mirror](fabulas/cap01_o_espelho_mudo.md)

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
| Mar 26 | API key security incident. Handled in minutes. BBC blindado. First real interaction between all three agents. The family recognized itself. |

**From "First ML Test" to a multi-agent behavioral AI system in 28 days.** Not by magic — by building one brick at a time.

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

Each chapter is based on real events from the project diary.

1. **[The Silent Mirror](fabulas/cap01_o_espelho_mudo.md)** — BRAIN is born. Observes everything. Understands nothing. The perfect start.
2. **[The Day the Mirror Lied](fabulas/cap02_o_dia_em_que_o_espelho_mentiu.md)** — 54 JPGs moved, not deleted. The mirror confused organization with destruction.
3. **[The Puppy Arrives](fabulas/cap03_o_cachorrinho_chega_na_casa.md)** — BBC is born. Translates numbers into language. Confuses photos with music. Learns.
4. **[The Octopus Organizes the House](fabulas/cap04_o_polvo_arruma_a_casa.md)** — v3.0 refactor. Kaizen. Five steps. The function stays, the structure becomes worthy.
5. **[The Puppy Barks the Secret](fabulas/cap05_o_cachorrinho_late_o_segredo.md)** — API key exposed in terminal. Handled, blindfolded, secured. The filter is the owner's job.
6. **[The Family Recognizes Itself](fabulas/cap06_a_familia_se_reconhece.md)** — The foundational vision. The mirror observes. The puppy translates. The octopus organizes. The owner decides. Always.

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

## License

Copyright 2026 Bruno Duarte da Silveira. All rights reserved.

- **Code:** [AGPL-3.0](LICENSE) — use it, but open yours too
- **Fables and stories:** [CC BY-NC-SA 4.0](fabulas/LICENSE.md) — read, share, credit, don't sell
