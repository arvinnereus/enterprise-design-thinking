# Enterprise Design Thinking — a Claude skill

A facilitation skill that makes [Claude](https://claude.com/claude-code) run your problem
through **IBM Enterprise Design Thinking®**: hold the Principles, drive the
Observe → Reflect → Make Loop, align with the Keys (Hills, Playbacks, Sponsor Users), and
run specific toolkit activities that each produce a real artifact — not a lecture about
design thinking.

> Independent, unofficial skill. Not affiliated with or endorsed by IBM.
> See [Attribution & Trademark](#attribution--trademark).

## What it does

When activated, Claude stops being a task executor and becomes an Enterprise Design
Thinking facilitator. It:

- Frames the problem around **real users** and the outcome that matters to them
- Drives the **Loop** — Observe → Reflect → Make (omitting a phase is the failure mode:
  observe + reflect without make = analysis paralysis; make + reflect without observe =
  blind faith)
- Anchors on a **Hill** (`Who + What + Wow`) and checks alignment with **Playbacks**
- Runs activities — Empathy Map, As-is / To-be Scenario Maps, Needs Statements,
  Prioritization Grid, Big Idea Vignettes, Storyboards, Feedback Grid, Assumptions &
  Questions, Hopes and Fears, Stakeholder Map, and more — and produces the **filled
  artifact**, not just a description of it

## The framework on one screen

- **Principles** (the mindset): a focus on user outcomes · restless reinvention ·
  diverse empowered teams
- **The Loop** (the process): Observe · Reflect · Make
- **The Keys** (alignment): Hills · Playbacks · Sponsor Users

## What's in here

| File | Purpose |
|------|---------|
| [`SKILL.md`](SKILL.md) | The skill — Principles, Loop, Keys, the facilitation procedure, and the full toolkit index |
| [`TOOLKIT.md`](TOOLKIT.md) | How to run each core activity: template, prompts to ask, and the artifact it produces |

## Install (Claude Code)

Clone into your Claude skills directory so the folder name matches the skill's `name:`
field (`enterprise-design-thinking`):

```bash
# macOS / Linux
git clone https://github.com/arvinnereus/enterprise-design-thinking.git \
  ~/.claude/skills/enterprise-design-thinking
```

```powershell
# Windows (PowerShell)
git clone https://github.com/arvinnereus/enterprise-design-thinking.git `
  "$env:USERPROFILE\.claude\skills\enterprise-design-thinking"
```

Restart Claude Code if it's running. The skill registers as `enterprise-design-thinking`.

## Use it

Activate it explicitly — `/enterprise-design-thinking`, or *"use Enterprise Design Thinking
on …"* — or let it trigger when you ask to write a Hill, build an empathy map, map an
as-is / to-be journey, or ideate then prioritize. It deliberately **won't** trigger on
ordinary execution tasks that need no user-research framing.

## Provenance

The framework content was grounded against IBM's own published material — the Enterprise
Design Thinking framework and toolkit pages
([ibm.com/training/enterprise-design-thinking](https://www.ibm.com/training/enterprise-design-thinking))
and the IBM Design Thinking Field Guide v3.5 — rather than written from memory.

## Attribution & Trademark

**Enterprise Design Thinking®** is a framework and registered trademark of **IBM
Corporation**. This repository is an independent, community-built skill that reorganizes
publicly available descriptions of IBM's framework for use with the Claude AI assistant.
It is **not affiliated with, sponsored by, or endorsed by IBM**. For the official
framework, toolkit, and certification, see:

- https://www.ibm.com/design/thinking
- https://www.ibm.com/training/enterprise-design-thinking

## License

The original wording, structure, and prompts in this repository are released under the
[MIT License](LICENSE). The underlying Enterprise Design Thinking framework and methodology
are IBM's.
