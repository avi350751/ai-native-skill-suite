# AI-Native Skill Suite

**Three career-stage agent skills that turn the ElevateXP AI transformation framework into practical coaching, diagnostics and decision support.**

> Use AI → Orchestrate AI → Reinvent with AI

---

## Why this repo exists

Most AI upskilling advice is one-size-fits-all: learn some prompts, try some tools, count the licences. [ElevateXP](project_sop.md) argues that this misses the point. Becoming "AI-native" looks very different for a graduate, a functional manager and a CEO. What they share is not tool fluency but **judgment**: knowing what AI should do, what humans should do, and how the work itself should change.

This repo packages that framework as three reusable **agent skills**, one per career stage. An AI assistant (Codex, Claude Code or any runtime that reads `SKILL.md` files) can load them to:

- coach individuals and teams from **AI Curious** to **AI Native**;
- produce grounded, evidence-based material instead of generic hype;
- keep a consistent voice and framework across a body of work. The suite was built to back a newsletter/article series on AI-native careers, and the skills are meant to be installed before drafting any article.

The source framework lives in [project_sop.md](project_sop.md). The design choices behind the translation are in [suite_overview.md](suite_overview.md).

---

## The framework in brief

### 3×3 model: scope × maturity

| | Use AI | Orchestrate AI | Reinvent with AI |
|---|---|---|---|
| **Individual** | AI-assisted productivity | AI-directed workflows | AI-native ways of working |
| **Team** | AI copilots | Human + AI coordination | AI-native teams |
| **Organization** | AI adoption | AI-enabled operating model | AI-native organization |

### Three horizons

| Horizon | Question |
|---|---|
| **H1 — Assist** | How can AI improve existing work? |
| **H2 — Redesign** | How should workflows change because AI exists? |
| **H3 — Reinvent** | What becomes possible that wasn't possible before? |

### Maturity ladder

```text
AI Curious → AI Assisted → AI Orchestrated → AI Native → AI Transformed
```

### From prompt engineering to loop engineering

```text
Goal → Context → Action → Observation → Evaluation → Correction → (next action)
```

Every skill pushes the user away from isolated prompts and toward observable, correctable human-AI loops.

---

## The skills

| Skill | Audience | Focus | Typical outputs |
|---|---|---|---|
| [`early-career-ai-native`](early-career-ai-native/SKILL.md) | Students, graduates, apprentices, career switchers, early-career staff from any field | AI literacy → AI-native execution | Capability diagnostic, 30/60/90-day roadmap, field-specific exercises, portfolio capstone with rubric |
| [`mid-career-ai-native`](mid-career-ai-native/SKILL.md) | Experienced specialists, managers, functional leaders | Domain + AI → AI-enabled leadership | Personal and team maturity profiles, workflow maps, prioritized use-case portfolio, pilot charter, adoption plan |
| [`cxo-ai-native`](cxo-ai-native/SKILL.md) | CEOs, CXOs, BU presidents, executive teams, boards | AI awareness → AI transformation and governance | Enterprise maturity profile, strategic thesis, stage-gated portfolio, target operating model, governance design, board narrative |

The skills hand off to each other. Early-career refers senior workflow ownership to mid-career, and mid-career refers enterprise strategy and board governance to CXO.

### Structure

Each skill follows the same layout:

```text
<skill>/
├── SKILL.md            # Frontmatter (name, description), principles, routing, core workflow, response contract
├── agents/openai.yaml  # Display name, short description, default prompt for agent UIs
└── references/         # Detailed playbooks, loaded only when the request needs them
```

`SKILL.md` stays short and routes to the reference files on demand, so the agent's context holds only what the task needs.

<details>
<summary><strong>Reference files by skill</strong></summary>

**early-career-ai-native**
- `diagnostic-and-roadmap.md`: learner profile, capability diagnostic, staged roadmap (Ground safely → Assist real work → Redesign a workflow → Work AI-natively), 30/60/90-day default
- `stream-map.md`: adaptations for 13 work streams (software, sciences, business, finance, law, health, arts, humanities, education, operations/trades, sales, HR, interdisciplinary) and for different starting points
- `practice-and-assessment.md`: practice design, portfolio capstone, rubric, workplace proof options

**mid-career-ai-native**
- `maturity-and-learning.md`: baseline profile, capability dimensions, learning journey (Domain + AI → Workflow designer → AI-enabled leader), readiness signals
- `function-playbooks.md`: use-case playbooks for 12 organizational functions
- `workflow-and-adoption.md`: workflow discovery, opportunity canvas, prioritization, human-AI loop design, pilot charter, adoption system, scale decision

**cxo-ai-native**
- `executive-diagnostic.md`: executive learning outcomes, alignment session, maturity dimensions, leadership archetypes
- `strategy-and-portfolio.md`: strategic thesis, portfolio categories and scoring, stage gates (Discovery → Pilot → Scale → Operate and renew), economics, board narrative
- `operating-model-and-governance.md`: decision rights, risk-tiered lifecycle, embedded governance, workforce, vendor posture, enterprise measures
- `cxo-role-lenses.md`: agendas tailored to CEO, COO, CIO/CTO, CDAO, CFO, CHRO, CMO/CRO, CPO/strategy, GC/risk, CISO, board and mission-led leaders

</details>

---

## Shared design principles

- **Outcome before technology.** Start from the problem and the desired result, not the tool.
- **AI-native ≠ maximum automation.** The goal isn't to turn everyone into an AI engineer.
- **Human authority is explicit.** Approval, escalation and accountability are designed in wherever consequences matter.
- **Evidence over activity.** Capability is shown through reproducible artifacts and measured outcomes, not prompt counts or licence usage.
- **Safe and honest use.** No confidential or regulated data in unapproved systems, and AI must not counterfeit competence.
- **Verify what changes.** Current tools, laws, standards and vendor claims are checked against primary sources and labelled when unverified.
- **"Do not proceed" is a valid answer.** Pilots have kill criteria, and scaling happens only from evidence.

---

## Installation

The skills use the standard `SKILL.md` format. Copy or symlink each skill folder into your agent's skills directory.

**Codex**

```bash
mkdir -p ~/.codex/skills
cp -R early-career-ai-native mid-career-ai-native cxo-ai-native ~/.codex/skills/
```

**Claude Code**

```bash
mkdir -p ~/.claude/skills
cp -R early-career-ai-native mid-career-ai-native cxo-ai-native ~/.claude/skills/
```

(Use `.claude/skills/` inside a project to scope the skills to that project.)

## Usage

Invoke a skill by name, or just describe the need and let the agent pick the matching skill from its description:

```text
Use $early-career-ai-native to assess my background and build an applied path from AI novice to AI-native contributor.

Use $mid-career-ai-native to turn my domain expertise into an AI-enabled workflow and adoption roadmap.

Use $cxo-ai-native to assess our enterprise AI maturity and define a value-led transformation agenda.
```

Example requests:

- *"I'm a final-year history student with no coding background. What does becoming AI-native look like for me?"*
- *"I run a 12-person finance ops team. Help me find and pilot one AI workflow worth scaling."*
- *"Prepare a board narrative on our AI portfolio, including what we should stop funding."*
- *"Draft a newsletter article on how the judgment layer changes for mid-career engineers."*

---

## Repository contents

| Path | Purpose |
|---|---|
| [project_sop.md](project_sop.md) | Source ElevateXP framework: 3×3 model, horizons, maturity model, judgment layer, roadmap, principles |
| [suite_overview.md](suite_overview.md) | How the SOP was translated into three skills, plus shared design choices |
| [early-career-ai-native/](early-career-ai-native/) | Early-career coaching skill |
| [mid-career-ai-native/](mid-career-ai-native/) | Mid-career coaching and adoption skill |
| [cxo-ai-native/](cxo-ai-native/) | Executive transformation and governance skill |

## Roadmap

The framework phase is complete. The broader ElevateXP roadmap in [project_sop.md](project_sop.md#roadmap) continues with structured assessments (individual, team, organization, 3×3 visualization), a transformation engine (opportunity and workflow mapping, roadmap generation, maturity tracking) and eventually an agentic ElevateXP with continuous assessment and outcome tracking.

## Contributing

Contributions are welcome, especially new work-stream or function playbooks, role lenses, assessment rubrics and worked examples. Please open an issue to discuss significant changes before submitting a pull request.

## License

No license has been chosen yet. Until one is added, all rights are reserved by the author.

---

**ElevateXP: from AI adoption to AI-native transformation.**
