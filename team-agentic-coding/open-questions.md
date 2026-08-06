# Open Questions

Seeded 2026-08-06. Unordered — add as they come up.

## Alignment & thinking

- **Grilling is single-player. What's the multiplayer version?** A grill surfaces one
  person's hidden assumptions. In a team, the assumptions that matter are the ones
  where two people silently disagree — and a 1:1 grill can't see those.
- Does the team align on the **spec**, or on the **domain model**, or on both? Which is
  the real unit of shared understanding?
- When two people's specs for the same feature disagree, is that a bug or a signal?

## Shared context

- `CLAUDE.md` / `AGENTS.md` / `CONTEXT.md` are per-repo files that everyone's agent
  reads. **Who owns them?** Who keeps them true?
- How do we stop context files from rotting? A stale `CONTEXT.md` is worse than none —
  it confidently misleads every agent on the team.
- Do we want one shared context, or per-person context layered on top of a shared base?

## Tool heterogeneity

- Claude Code, Codex, Antigravity — different config formats, different capabilities,
  different failure modes. **Do we standardize on one, or stay polyglot?**
- If polyglot: what's the lowest common denominator we write context/specs against?
- Does a skill/prompt written for one agent transfer to another, or do we maintain N copies?

## Throughput & bottlenecks

- If everyone ships 3× more code, **review becomes the bottleneck.** What gives?
- Who reviews agent-written code — a human, another agent, or both? In what order?
- More parallel branches → more merge conflicts. Does that scale or fall over?

## Ownership & understanding

- If an agent wrote it and a human approved it, **who owns the bug?**
- How do we prevent a team-wide version of "I shipped it but I don't understand it"?
- Does agentic tooling make onboarding faster, or does it hide the codebase from newcomers
  and make it slower in month three?

## Process mechanics

- What does a **standup** look like when half the work was done by agents overnight?
- Do tickets get written by humans, by agents, or by agents-from-human-conversation?
- Where does pairing fit? Is "two humans + one agent" a real format or a worse version of both?
