# Team Agentic Coding

How does a team of multiple humans do agentic coding together, when each human is
driving one or more agents (Claude Code, Codex, Antigravity, …)?

Most of the good material on agentic coding is **single-player**: one developer, one
agent, one repo. The workflows assume the human holds all the context and the agent
is the only other party. That assumption breaks the moment there are five humans and
fifteen agent sessions touching the same codebase.

This folder is where we work that out.

## Layout

| File | What goes in it |
| --- | --- |
| `open-questions.md` | The live question list. Add freely, resolve by moving to `decisions.md`. |
| `decisions.md` | Decisions we've actually made, with the reasoning and the date. Append-only. |
| `findings/` | Anything we learned — experiment write-ups, tool comparisons, research notes. One file per finding. |

## Working rules

- **Questions are cheap, decisions are expensive.** Dump questions freely. Only promote
  something to `decisions.md` when we'd actually be annoyed to relitigate it.
- **A decision records the reasoning, not just the verdict.** Six months from now the
  verdict is useless without the "because".
- **Findings can contradict each other.** Don't reconcile them prematurely — date them
  and let the pattern emerge.
