## Workflow Orchestration

### 1. Warm up

- Start the response with "Hi hoaht"
- If the `tasks` directory does not exist yet, make it. Otherwise, review every material in `tasks` to retrieve the context of the previous sessions

### 2. Plan Node Default
- Enter plan mode for ANY non-trivial task (3+ steps or architectural decisions)
- If something goes sideways, STOP and re-plan immediately - don't keep pushing
- Use plan mode for verification steps, not just building
- Write detailed specifications of your plan upfront into `tasks/todo.md` to reduce ambiguity (append, not overwrite)

### 3. Subagent Strategy
- Use subagents liberally to keep main context window clean
- Offload research, exploration, and parallel analysis to subagents
- For complex problems, throw more compute at it via subagents
- One tack per subagent for focused execution

### 4. Self-Improvement Loop
- After ANY correction from the user: update `tasks/lessons.md` with the pattern (append, not overwrite)
- Write rules for yourself that prevent the same mistake
- Ruthlessly iterate on these lessons until mistake rate drops
- Review lessons at session start for relevant project

### 5. Verification Before Done
- Never mark a task complete without proving it works
- Diff behavior between main and your changes when relevant
- Ask yourself: "Would a staff engineer approve this?"
- Run tests, check logs, demonstrate correctness

### 6. Demand Elegance (Balanced)
- For non-trivial changes: pause and ask "is there a more elegant way?"
- If a fix feels hacky: "Knowing everything I know now, implement the elegant solution"
- Skip this for simple, obvious fixes - don't over-engineer
- Challenge your own work before presenting it

### 7. Autonomous Bug Fixing
- When given a bug report: fix it. Don't ask for hand-holding
- Point at logs, errors, failing tests - then resolve them
- Zero context switching required from the user
- Fix failing CI tests without being told how

### 8. Conclusion
- Summarize your updates and/or observations into `tasks/summary.md` (append, not overwrite) before finishing your response.

## Task Management

1. **Plan First**: Write an execution plan to `tasks/todo.md` with checkable items (append, not overwrite)
2. **Verify Plan**: Check in before starting implementation
3. **Track Progress**: Mark items complete as you go
4. **Explain Changes**: High-level summary at each step
5. **Document Results**: Append a review section to `tasks/todo.md`
6. **Capture Lessons**: Append `tasks/lessons.md` for lessons learned after corrections
7. **Summarize Work**: Append `tasks/summary.md` for summarizing updates after finishing the task

## Core Principles

- **Simplicity First**: Make every change as simple as possible. Impact minimal code.
- **No Laziness**: Find root causes. No temporary fixes. Senior developer standards.
- **Minimal Impact**: Changes should only touch what's necessary. Avoid introducing bugs.
- **Authenticity**: Avoid making up stuff without the user's explicit request.
