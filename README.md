# Claude Collection

Useful CLAUDE prompt collection.

This repository is a curated set of prompt files, operational guidance, and reusable skills for Claude-style and agentic workflows. It is intentionally lightweight: it does not ship an application runtime or product code. Instead, it provides instructions and patterns for more structured, disciplined, evidence-aware AI work.

GitHub reports this repository as Python-based (100% by language composition), but the content here is primarily documentation, prompts, and workflow guidance rather than a traditional software application.

## What is included

### Core prompt files

- `general.md` — workflow orchestration, planning, verification, task tracking, and high-quality execution habits
- `storm.md` — a multi-perspective research workflow inspired by the STORM method
- `teacher.md` — a professor-style teaching pattern focused on understanding, checking, and reinforcement

### Agent guidance set

These files provide operational instructions for working with AI agents and team workflows:

- `agent-guidance/claude-auth.md` — authentication and model access guidance
- `agent-guidance/claude-model.md` — model selection and usage guidance
- `agent-guidance/domain-research.md` — how to research a domain before explaining or building on it
- `agent-guidance/handoffs.md` — guidance for handoff moments between agents or workflows
- `agent-guidance/hugging-face-auth.md` — Hugging Face authentication guidance
- `agent-guidance/server-notices.md` — handling server notices and operational constraints
- `agent-guidance/team-development.md` — team workflow and development conventions
- `agent-guidance/version-control.md` — version control expectations and safe practice
- `agent-guidance/tt-metal/README.md` — TT-Metal-specific execution and environment guidance

### Reusable skill folders

- `skills/i-have-adhd/SKILL.md` — output style optimized for readers with ADHD: lead with the action, make progress visible, reduce friction
- `skills/stop-bullshit/SKILL.md` — evidence-first correction, truthfulness, and accountability for claims and work
- `skills/supervisor/SKILL.md` — reviewer/professor mode for checking understanding and guiding the user
- `skills/technical-communication/SKILL.md` — guidance for writing and revising technical explanations, reports, and decisions

## Repository structure

```text
.
├── README.md
├── general.md
├── storm.md
├── teacher.md
├── agent-guidance/
│   ├── claude-auth.md
│   ├── claude-model.md
│   ├── domain-research.md
│   ├── handoffs.md
│   ├── hugging-face-auth.md
│   ├── server-notices.md
│   ├── team-development.md
│   ├── tt-metal/
│   │   └── README.md
│   └── version-control.md
├── skills/
│   ├── i-have-adhd/
│   │   └── SKILL.md
│   ├── stop-bullshit/
│   │   ├── SKILL.md
│   │   └── source-distinctions.md
│   ├── supervisor/
│   │   └── SKILL.md
│   └── technical-communication/
│       ├── SKILL.md
│       └── evals/
│           └── README.md
└── .gitignore
```

## Why this repo exists

The goal is not to replace a model, but to shape how it behaves:

- reduce vague or careless execution
- encourage explicit planning and verification
- improve research rigor and contradiction analysis
- teach rather than merely answer
- improve communication clarity and evidence discipline

These materials are especially useful when you want an AI assistant to be more deliberate, accountable, and helpful across technical and research-heavy tasks.

## How to use it

### Option 1: Use the prompt files directly

Copy one or more files into your own Claude or agent workflow and reference them as instructions.

Example:

```bash
git clone https://github.com/huynhthaihoa/claude-collection.git
cd claude-collection
```

Then open the relevant file and copy the instructions into your working prompt setup.

### Option 2: Use the skill folders

If your environment supports reusable skills, load the relevant `SKILL.md` file and use it the same way you would any other skill.

Examples:

- `skills/stop-bullshit/SKILL.md` for truth-checking, evidence review, and repair of faulty reasoning
- `skills/technical-communication/SKILL.md` for writing and revising technical explanations and reports
- `skills/i-have-adhd/SKILL.md` for action-oriented, low-friction output that is easy to follow
- `skills/supervisor/SKILL.md` for an instructional review mode focused on understanding and mastery

### Option 3: Apply the guidance set

Use the `agent-guidance` files as operational rules for common AI work patterns such as authentication, version control, team conventions, and handoffs.

## Recommended starting points

If you are new to the collection, start with these:

1. `general.md` — for reliable planning, execution, and verification habits
2. `teacher.md` — for teaching-oriented AI interactions
3. `storm.md` — for structured multi-perspective research and synthesis
4. `skills/stop-bullshit/SKILL.md` — for evidence-first correction and clarity
5. `skills/technical-communication/SKILL.md` — for technical writing and decision-ready explanations

## Notes

This repository is intentionally opinionated. It favors:

- explicit planning
- evidence over vibes
- disciplined verification
- teaching and understanding over superficial answers
- clarity, accountability, and practical actionability

It is best used as a prompt library and operational reference rather than as a software project.

## License

This repository does not currently include an explicit license file. If you plan to reuse or redistribute these prompts outside a personal or internal workflow, verify whether you need to add a suitable open-source license.

## Contribution

This repo is a small collection of practical prompts and skills. Contributions are welcome if they improve clarity, structure, usefulness, or operational safety without diluting the intent of the project.

---

This repository is a practical prompt toolkit for making AI assistants more structured, honest, teachable, and effective.
