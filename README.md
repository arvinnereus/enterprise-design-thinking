# Enterprise Design Thinking — a Claude skill

A facilitation skill that makes [Claude](https://claude.com/claude-code) run your problem
through **IBM Enterprise Design Thinking®**: hold the Principles, drive the
Observe → Reflect → Make Loop, align with the Keys (Hills, Playbacks, Sponsor Users), and
run specific toolkit activities that each produce a real artifact — not a lecture about
design thinking.

> **Enterprise Design Thinking® was created and is owned by IBM Corporation** and is a
> registered trademark of IBM. This is an independent, unofficial skill based on that
> concept — not affiliated with or endorsed by IBM, and claiming no ownership of the
> framework. See [Credits & Attribution](#credits--attribution).

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

## Simulated-session mode

When you bring a topic but no real users to interview, the skill can run a
**full Observe → Reflect → Make loop as a simulated multi-voice session**:

1. **Cast** — assembles a diverse facilitation team and ~5 Sponsor Users whose
   backgrounds represent the range of people affected by the problem
2. **Observe (to saturation)** — runs interview rounds with each Sponsor User,
   looping until consecutive rounds produce no new themes (saturation, not a fixed
   count)
3. **Reflect** — synthesises findings into an Empathy Map, Needs Statements, and
   How-Might-We questions; flags any mirror-risk (where all voices converge too
   neatly and may reflect the prompt rather than genuine diversity)
4. **Make** — produces Hills, a To-be Scenario, and an architecture or action plan
   grounded in the synthesised findings
5. **Stress-test** — an adversarial pass challenges each Hill and assumption before
   the session closes

**Hard honesty rule:** every finding from a simulated session is labelled a
*hypothesis to validate with real users* — not research. The skill will say so
explicitly and will not present simulated voices as validated evidence.

Trigger it the same way as single-pass facilitation — `/enterprise-design-thinking`
or *"use Enterprise Design Thinking on …"* — and add *"run a simulated session"* or
*"cast Sponsor Users"* if you want the full multi-voice loop rather than coached
facilitation.

## Provenance

The framework content was grounded against IBM's own published material — the Enterprise
Design Thinking framework and toolkit pages
([ibm.com/training/enterprise-design-thinking](https://www.ibm.com/training/enterprise-design-thinking))
and the IBM Design Thinking Field Guide v3.5 — rather than written from memory.

## Credits & Attribution

**Enterprise Design Thinking® was created and is owned by IBM Corporation** (IBM Design).
"Enterprise Design Thinking" is a **registered trademark of IBM**, and the framework — its
Principles, the Loop (Observe / Reflect / Make), the Keys (Hills, Playbacks, Sponsor
Users), and the activity toolkit — is the intellectual property of IBM. The IBM Design
Thinking Field Guide is **© IBM Corporation**.

This repository is an **independent, unofficial** Claude skill that reorganizes publicly
available descriptions of IBM's framework so it can be used with the Claude AI assistant.
It claims **no ownership** of the framework, is **not affiliated with, sponsored by, or
endorsed by IBM**, and is offered purely as a practitioner aid. **All credit for the
methodology belongs to IBM.**

For the official framework, toolkit, certification, and Field Guide, see:

- https://www.ibm.com/design/thinking
- https://www.ibm.com/training/enterprise-design-thinking

See also the [`NOTICE`](NOTICE) file.

## License

The MIT License in [`LICENSE`](LICENSE) covers **only** the original wording, structure,
and prompts authored for this skill. It does **not** extend to the Enterprise Design
Thinking framework or trademark, which remain the property of IBM. See [`NOTICE`](NOTICE).
