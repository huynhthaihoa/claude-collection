# Claude Collection

Useful CLAUDE prompt collection.

A curated set of instruction files and reusable agent skills designed to make Claude-style assistants more disciplined, thoughtful, and effective across planning, research, teaching, debugging, and technical communication.

This repository is intentionally lightweight: it does not ship application code or a runtime. Instead, it provides prompt assets that can be copied into a Claude/agent workflow, integrated into a custom skill system, or used as inspiration for your own prompts.

## What is included

### Core prompt files

- `general.md` — broad operating guidance for task management, planning, verification, and execution discipline
- `storm.md` — a Stanford-inspired multi-perspective research workflow for synthesizing complex topics
- `teacher.md` — a tutoring mode focused on conceptual understanding and checking what the learner truly knows

### Reusable skill folders

- `skills/i-have-adhd/` — output style tuned for readers with ADHD: clear next action, visible progress, and reduced cognitive friction
- `skills/stop-bullshit/` — evidence-first guidance for truthfulness, correction, and accountable work
- `skills/technical-communication/` — help for producing clear technical explanations and decision-ready documentation

## Repository structure

```text
.
├── general.md
├── storm.md
├── teacher.md
├── skills/
│   ├── i-have-adhd/
│   │   └── SKILL.md
│   ├── stop-bullshit/
│   │   ├── SKILL.md
│   │   └── source-distinctions.md
│   └── technical-communication/
│       └── SKILL.md
└── README.md
```

## Why this repo exists

The goal is not to replace a model, but to shape how it behaves:

- reduce vague or careless execution
- encourage explicit planning and verification
- improve research rigor and contradiction analysis
- teach rather than merely answer
- keep communication precise and evidence-aware

These files are especially helpful when you want an AI assistant to be more structured, less fluffy, and more accountable in its reasoning and output.

## How to use it

### Option 1: Use the prompt files directly

Copy one or more files into your own Claude/agent environment and reference them as instructions.

Example:

```bash
git clone https://github.com/huynhthaihoa/claude-collection.git
cd claude-collection
```

Then open any file and copy the relevant instructions into your prompt setup.

### Option 2: Use the skill folders

If your environment supports reusable skills, load the relevant `SKILL.md` file and use it in the same way you would any other skill.

Examples:

- `skills/stop-bullshit/SKILL.md` for debunking weak claims and repairing bad reasoning
- `skills/technical-communication/SKILL.md` for writing and revising engineering explanations
- `skills/i-have-adhd/SKILL.md` for action-oriented, cognitively friendly output

## Recommended starting points

If you are new to the collection, start with these:

1. `general.md` — for good habits in task execution and verification
2. `teacher.md` — if you want the assistant to help someone understand deeply
3. `storm.md` — for structured research and synthesis across perspectives
4. `skills/stop-bullshit/SKILL.md` — for high-trust, evidence-based answering

## Notes

This repository is intentionally opinionated. It favors:

- explicit planning
- evidence over vibes
- clear next actions
- teaching and understanding over surface-level answers
- disciplined reasoning and communication

It is best used as a prompt library and design reference rather than a software project.

## License

No explicit license file is included in this repository as of now. If you plan to reuse these prompts in a commercial or public setting, check whether you need to add an appropriate license before distributing them.

## Contribution

This repo is a small collection of practical prompts and skills. Contributions are welcome if they improve clarity, structure, or usefulness without diluting the intent of the project.

---

This repository is a practical prompt toolkit for making AI assistants more structured, honest, teachable, and effective.
